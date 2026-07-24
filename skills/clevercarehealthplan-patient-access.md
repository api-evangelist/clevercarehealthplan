---
name: Clever Care patient access (claims and coverage)
description: Authenticate a member with SMART-on-FHIR and read their Patient, Coverage, and ExplanationOfBenefit (claims) data.
api: openapi/clevercarehealthplan-fhir-openapi.yml
operations: [searchPatient, readPatient, searchCoverage, searchExplanationOfBenefit, readExplanationOfBenefit]
---

# Clever Care patient access

Read a Clever Care Health Plan member's own data via the FHIR R4 Patient Access API (CMS-9115-F). All Patient Access resources are secured.

## Auth
1. Obtain an access token via SMART-on-FHIR OAuth 2.0 authorization code flow (PKCE, `S256`):
   - authorize: `https://fhir-portal.clevercarehealthplan.com/oauth2/authorize`
   - token: `https://fhir-portal.clevercarehealthplan.com/oauth2/token`
   - request scopes: `openid launch/patient patient/*.cruds` (or `user/*.cruds`).
2. Send the token as `Authorization: Bearer <token>`. Base URL: `https://fhir.clevercarehealthplan.com/r4`. Accept `application/fhir+json`.

## Steps
1. `searchPatient` (or `readPatient` with the id from the `launch/patient` context) to resolve the member.
2. `searchCoverage` to list the member's plan coverage.
3. `searchExplanationOfBenefit` with the required `patient` parameter to list claims (CARIN Blue Button C4BB profiles). Use `readExplanationOfBenefit` for a single claim.

## Rules
- All interactions are read-only (`read`/`search-type`); there are no writes, so no idempotency key is needed.
- Errors return a FHIR `OperationOutcome` (`issue[].severity`, `code`, `diagnostics`). `401` = missing/invalid token; `403` = insufficient scope; `404` = unknown id.
- Page through results using `Bundle.link` entries with `relation: next`.
