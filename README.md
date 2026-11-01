# USAspending.gov

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

USAspending.gov is the official open data source of federal spending information operated by the U.S. Department of the Treasury's Bureau of the Fiscal Service, implementing the DATA Act's transparency mandate. The underlying USAspending API (api.usaspending.gov) is a free, public, unauthenticated REST API that exposes federal contracts, grants, loans, direct payments, and other financial assistance awards, along with agency budgets, federal account and Treasury Account Symbol data, recipient profiles, and COVID-19 / disaster emergency relief spending. Most search and listing endpoints accept a POST with a JSON filter object rather than query parameters, given the complexity of the filter combinations; simpler lookup endpoints use GET with path parameters. The API and the usaspending-api server are open source.

**Areas:** Government · Federal Spending · Open Data · Contracts · Grants · DATA Act · Transparency · Public Sector · Government Data

## USAspending.gov on APIs.io

Everything profiled for USAspending.gov is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/usaspending/](https://apis.io/providers/usaspending/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [USAspending.gov Agency API](https://apis.io/apis/usaspending/usaspending-agency-api/) — Per-agency profile, budget, and award data.
- [USAspending.gov Awards Search API](https://apis.io/apis/usaspending/usaspending-awards-search-api/) — Advanced search and filtering across award and subaward spending.
- [USAspending.gov Budget Functions API](https://apis.io/apis/usaspending/usaspending-budget-functions-api/) — Federal budget functional classification reference data.
- [USAspending.gov Bulk Download API](https://apis.io/apis/usaspending/usaspending-bulk-download-api/) — Asynchronous bulk CSV/TSV/text export of filtered spending data.
- [USAspending.gov Disaster API](https://apis.io/apis/usaspending/usaspending-disaster-api/) — Disaster and emergency (including COVID-19) supplemental funding data.
- [USAspending.gov Federal Accounts API](https://apis.io/apis/usaspending/usaspending-federal-accounts-api/) — Federal account and Treasury Account Symbol (TAS) data.
- [USAspending.gov Recipient API](https://apis.io/apis/usaspending/usaspending-recipient-api/) — Recipient (awardee) profile and search data.
- [USAspending.gov References API](https://apis.io/apis/usaspending/usaspending-references-api/) — Reference and typeahead/autocomplete lookup data.
- [USAspending.gov Subawards API](https://apis.io/apis/usaspending/usaspending-subawards-api/) — Subaward (pass-through award) listings scoped to a prime award.
- [USAspending.gov](https://apis.io/apis/usaspending/usaspendinggov/) — US federal spending data

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Usaspending Agentic Access](https://apis.io/agentic-access/usaspending/usaspending-agentic-access/)

#### Collections (10)

Postman and Open Collection request collections.

- [USAspending API](https://apis.io/collections/usaspending/open-usaspending/)
- [USAspending Agency API](https://apis.io/collections/usaspending/open-usaspending-agency-api/)
- [USAspending Agency Awards Search API](https://apis.io/collections/usaspending/open-usaspending-awards-search-api/)
- [USAspending Agency Budget Functions API](https://apis.io/collections/usaspending/open-usaspending-budget-functions-api/)
- [USAspending Agency Bulk Download API](https://apis.io/collections/usaspending/open-usaspending-bulk-download-api/)
- [USAspending Agency Disaster API](https://apis.io/collections/usaspending/open-usaspending-disaster-api/)
- [USAspending Agency Federal Accounts API](https://apis.io/collections/usaspending/open-usaspending-federal-accounts-api/)
- [USAspending Agency Recipient API](https://apis.io/collections/usaspending/open-usaspending-recipient-api/)
- [USAspending Agency References API](https://apis.io/collections/usaspending/open-usaspending-references-api/)
- [USAspending Agency Subawards API](https://apis.io/collections/usaspending/open-usaspending-subawards-api/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Usaspending Domain Security](https://apis.io/security/usaspending/usaspending-domain-security/)

#### Rate limits (1)

Published request limits.

- [Usaspending Rate Limits](https://apis.io/rate-limits/usaspending/usaspending-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.usaspending.gov)
- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [Blog](https://www.usaspending.gov/blog/)
- [GitHub](https://github.com/fedspendingtransparency)

## API Evangelist rating

**Kin Score 21.3** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 45.4 |
| Contract governance | 0.0 |
| Operational transparency | 10.5 |
| Developer ergonomics | 19.0 |
| Access clarity | 0.0 |

**Agent readiness 17.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 5.9** — Government & Public Sector

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/usaspending/](https://apis.io/providers/usaspending/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for USAspending.gov: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/usaspending/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
