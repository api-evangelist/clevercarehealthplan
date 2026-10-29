# Clever Care Health Plan

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Clever Care Health Plan is a California Medicare Advantage (HMO and HMO C-SNP) insurer that blends Eastern and Western medicine for seniors. For developers it publishes an HL7 FHIR R4 (4.0.1) API implementing the CMS Interoperability and Patient Access final rule (CMS-9115-F): a secured Patient Access API (Patient, Coverage, and CARIN Blue Button ExplanationOfBenefit) protected with SMART-on-FHIR OAuth 2.0 / OpenID Connect, plus public, rate-limited Provider Directory and Drug Formulary APIs. The FHIR server runs on WSO2 Open Healthcare with a developer portal for app registration and API subscription.

**Areas:** Company · Healthcare · Health Insurance · Medicare Advantage · FHIR · Interoperability · Patient Access · Provider Directory · Drug Formulary · CMS-9115-F

## Clever Care Health Plan on APIs.io

Everything profiled for Clever Care Health Plan is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/clevercarehealthplan/](https://apis.io/providers/clevercarehealthplan/)** — or go straight to one of the APIs or properties below.

### APIs (3)

- [Clever Care Health Plan Drug Formulary API](https://apis.io/apis/clevercarehealthplan/clevercarehealthplan-drug-formulary-api/) — Public (rate limited) drug formulary resources
- [Clever Care Health Plan Patient Access API](https://apis.io/apis/clevercarehealthplan/clevercarehealthplan-patient-access-api/) — Secured (OpenID Connect / OAuth 2.0) member data resources
- [Clever Care Health Plan Provider Directory API](https://apis.io/apis/clevercarehealthplan/clevercarehealthplan-provider-directory-api/) — Public (rate limited) provider directory resources

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [clevercarehealthplan-fhir](https://apis.io/servers/clevercarehealthplan/clevercarehealthplan-fhir/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Clevercarehealthplan Agentic Access](https://apis.io/agentic-access/clevercarehealthplan/clevercarehealthplan-agentic-access/)

#### Collections (3)

Postman and Open Collection request collections.

- [Clever Care Health Plan FHIR R4 Drug Formulary API](https://apis.io/collections/clevercarehealthplan/open-clevercarehealthplan-drug-formulary-api/)
- [Clever Care Health Plan FHIR R4 Drug Formulary Patient Access API](https://apis.io/collections/clevercarehealthplan/open-clevercarehealthplan-patient-access-api/)
- [Clever Care Health Plan FHIR R4 Drug Formulary Provider Directory API](https://apis.io/collections/clevercarehealthplan/open-clevercarehealthplan-provider-directory-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Clevercarehealthplan Fhir Overlay](https://apis.io/overlays/clevercarehealthplan/clevercarehealthplan-fhir-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Clevercarehealthplan Authentication](https://apis.io/security/clevercarehealthplan/clevercarehealthplan-authentication/)
- [Clevercarehealthplan Domain Security](https://apis.io/security/clevercarehealthplan/clevercarehealthplan-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Clevercarehealthplan Scopes](https://apis.io/scopes/clevercarehealthplan/clevercarehealthplan-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://clevercarehealthplan.com)
- [Documentation](https://fhir-portal.clevercarehealthplan.com/api-docs/)
- [Getting started](https://clevercarehealthplan.com/fhir-api-developer-resources/)
- [API reference](https://fhir-portal.clevercarehealthplan.com/api-docs/)
- [Sign up](https://fhir-portal.clevercarehealthplan.com/devportal)
- [Compliance](https://clevercarehealthplan.com/medicare-compliance/)
- [Terms of service](https://clevercarehealthplan.com/terms-of-use/)
- [Privacy policy](https://clevercarehealthplan.com/privacy-practices/)

## API Evangelist rating

**Kin Score 36.0** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 44.5 |
| Contract governance | 18.2 |
| Operational transparency | 0.0 |
| Developer ergonomics | 39.9 |
| Access clarity | 13.2 |

**Agent readiness 27.7** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | na |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 43.8** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/clevercarehealthplan/](https://apis.io/providers/clevercarehealthplan/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Clever Care Health Plan: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/clevercarehealthplan/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
