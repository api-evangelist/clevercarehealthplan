---
name: Clever Care provider directory search
description: Search the public Clever Care provider directory for organizations, practitioners, roles, locations, and services.
api: openapi/clevercarehealthplan-fhir-openapi.yml
operations: [searchOrganization, searchPractitioner, searchPractitionerRole, searchLocation, searchHealthcareService, searchInsurancePlan]
---

# Clever Care provider directory search

Query the public (rate-limited, no auth) FHIR R4 Provider Directory API.

## Access
- Base URL: `https://fhir.clevercarehealthplan.com/r4`, Accept `application/fhir+json`. No token required; endpoints are rate limited.

## Steps
1. `searchPractitioner` to find clinicians (filter with `_id`, `_lastUpdated`, `_profile`).
2. `searchPractitionerRole` to resolve a practitioner's affiliations, locations, and services.
3. `searchOrganization` for groups/facilities; `searchLocation` for physical sites.
4. `searchHealthcareService` for services offered; `searchInsurancePlan` for the plans a provider participates in.

## Rules
- Read-only search + read interactions only.
- Follow `Bundle.link` `relation: next` for pagination.
- On `429` (throttled `OperationOutcome`), back off and retry.
