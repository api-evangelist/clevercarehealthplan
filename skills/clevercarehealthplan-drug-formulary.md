---
name: Clever Care drug formulary lookup
description: Look up covered drugs and formulary lists from the public Clever Care Drug Formulary API.
api: openapi/clevercarehealthplan-fhir-openapi.yml
operations: [searchMedicationKnowledge, readMedicationKnowledge, searchList, readList]
---

# Clever Care drug formulary lookup

Query the public (rate-limited, no auth) FHIR R4 Drug Formulary API.

## Access
- Base URL: `https://fhir.clevercarehealthplan.com/r4`, Accept `application/fhir+json`. No token required.

## Steps
1. `searchMedicationKnowledge` to find formulary drugs (filter with `_id`, `_lastUpdated`, `_profile`); `readMedicationKnowledge` for one drug.
2. `searchList` to retrieve formulary drug lists (tiers/coverage groupings); `readList` for a specific list.

## Rules
- Read-only search + read interactions only.
- Errors are FHIR `OperationOutcome`. Handle `429` with backoff.
- Paginate via `Bundle.link` `relation: next`.
