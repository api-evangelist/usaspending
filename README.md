# USAspending.gov (usaspending)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

USAspending.gov is the official open data source of U.S. federal spending information, operated by the Treasury Department's Bureau of the Fiscal Service to implement the DATA Act's transparency mandate. The underlying USAspending API (`api.usaspending.gov`) is a free, public, unauthenticated REST API that exposes federal contracts, grants, loans, direct payments, and other financial assistance awards, along with agency budgets, federal account and Treasury Account Symbol data, recipient profiles, and COVID-19 / disaster emergency relief spending. Most search and listing endpoints accept a `POST` with a JSON filter object rather than query parameters, given the complexity of the filter combinations; simpler lookup endpoints use `GET` with path parameters. The API and the `usaspending-api` server are open source (CC0 / public domain).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/usaspending/refs/heads/main/apis.yml)

## Tags

- Government
- Federal Spending
- Open Data
- Contracts
- Grants
- DATA Act
- Transparency
- Public Sector

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### USAspending Awards Search API

Advanced search across federal award spending (contracts, IDVs, grants, loans, direct payments, other financial assistance). Accepts a complex JSON filter object (award type, agency, recipient, time period, place of performance, NAICS/PSC, keyword, and more) plus a requested field list, and returns paged, sortable award or subaward records. Powers the USAspending.gov Advanced Search page, spending-by-category, spending-by-geography, and spending-over-time breakdowns.

- **Human URL:** [https://api.usaspending.gov/docs/endpoints](https://api.usaspending.gov/docs/endpoints)
- **Base URL:** `https://api.usaspending.gov/api/v2`

#### Properties

- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [API Reference](https://github.com/fedspendingtransparency/usaspending-api/blob/master/usaspending_api/api_contracts/contracts/v2/search/spending_by_award.md)
- [OpenAPI](openapi/usaspending-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/usaspending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/usaspending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USAspending Agency API

Per-agency profile data keyed by toptier agency code - mission, website, budgetary resources, obligated and outlay amounts, awards, sub-agencies, and Disaster Emergency Fund Code (DEFC) participation for a given fiscal year. Powers the USAspending.gov agency profile pages.

- **Human URL:** [https://api.usaspending.gov/docs/endpoints](https://api.usaspending.gov/docs/endpoints)
- **Base URL:** `https://api.usaspending.gov/api/v2`

#### Properties

- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [API Reference](https://github.com/fedspendingtransparency/usaspending-api/blob/master/usaspending_api/api_contracts/contracts/v2/agency/toptier_code.md)
- [OpenAPI](openapi/usaspending-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/usaspending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/usaspending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USAspending Recipient API

Recipient (awardee) profile data - list and search recipients by keyword, UEI, or (deprecated) DUNS, sorted by award amount, plus per-recipient award breakdowns by award type and state. Powers the USAspending.gov recipient profile pages.

- **Human URL:** [https://api.usaspending.gov/docs/endpoints](https://api.usaspending.gov/docs/endpoints)
- **Base URL:** `https://api.usaspending.gov/api/v2`

#### Properties

- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [API Reference](https://github.com/fedspendingtransparency/usaspending-api/blob/master/usaspending_api/api_contracts/contracts/v2/recipient.md)
- [OpenAPI](openapi/usaspending-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/usaspending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/usaspending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USAspending Federal Account API

Federal account and child Treasury Account Symbol (TAS) data for a given fiscal year - account title, parent agency and bureau, and aggregated obligated, gross outlay, and budgetary resources amounts. Powers the USAspending.gov federal account landing and detail pages.

- **Human URL:** [https://api.usaspending.gov/docs/endpoints](https://api.usaspending.gov/docs/endpoints)
- **Base URL:** `https://api.usaspending.gov/api/v2`

#### Properties

- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [API Reference](https://github.com/fedspendingtransparency/usaspending-api/blob/master/usaspending_api/api_contracts/contracts/v2/federal_accounts/account_number.md)
- [OpenAPI](openapi/usaspending-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/usaspending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/usaspending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USAspending Budget Function API

Reference listings of the federal budget's functional classification - budget functions and budget subfunctions (for example, National Defense, Health, Income Security) used to categorize and filter agency budgetary resources across the federal government.

- **Human URL:** [https://api.usaspending.gov/docs/endpoints](https://api.usaspending.gov/docs/endpoints)
- **Base URL:** `https://api.usaspending.gov/api/v2`

#### Properties

- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [API Reference](https://github.com/fedspendingtransparency/usaspending-api/blob/master/usaspending_api/api_contracts/contracts/v2/budget_functions/list_budget_functions.md)
- [OpenAPI](openapi/usaspending-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/usaspending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/usaspending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USAspending Disaster/Emergency Funding (COVID-19) API

Funding and spending detail for emergency and disaster supplemental appropriations, tracked by Disaster Emergency Fund Code (DEFC) - including the CARES Act and other COVID-19 relief legislation. Breaks down total budget authority, obligations, and outlays by agency, award, CFDA program, federal account, object class, recipient, and geography.

- **Human URL:** [https://api.usaspending.gov/docs/endpoints](https://api.usaspending.gov/docs/endpoints)
- **Base URL:** `https://api.usaspending.gov/api/v2`

#### Properties

- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [API Reference](https://github.com/fedspendingtransparency/usaspending-api/blob/master/usaspending_api/api_contracts/contracts/v2/disaster/overview.md)
- [OpenAPI](openapi/usaspending-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/usaspending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/usaspending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USAspending Bulk Download API

Asynchronous bulk export of filtered award, account, and transaction data as zipped CSV, TSV, or pipe-delimited text files. A request kicks off zip-file generation on the backend; a companion status endpoint is polled until the file is ready for download. Also lists agencies and monthly generated files available for download. Powers the USAspending.gov Custom Award Data Download page.

- **Human URL:** [https://api.usaspending.gov/docs/endpoints](https://api.usaspending.gov/docs/endpoints)
- **Base URL:** `https://api.usaspending.gov/api/v2`

#### Properties

- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [API Reference](https://github.com/fedspendingtransparency/usaspending-api/blob/master/usaspending_api/api_contracts/contracts/v2/bulk_download/awards.md)
- [OpenAPI](openapi/usaspending-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/usaspending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/usaspending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USAspending References & Autocomplete API

Reference and typeahead data used to build and validate search filters across the rest of the API - toptier agency listings with budgetary-resources share, plus autocomplete lookups for awarding/funding agencies and sub-agency offices, recipients, CFDA assistance listings, NAICS and PSC codes, locations, and glossary terms.

- **Human URL:** [https://api.usaspending.gov/docs/endpoints](https://api.usaspending.gov/docs/endpoints)
- **Base URL:** `https://api.usaspending.gov/api/v2`

#### Properties

- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [API Reference](https://github.com/fedspendingtransparency/usaspending-api/blob/master/usaspending_api/api_contracts/contracts/v2/references/toptier_agencies.md)
- [OpenAPI](openapi/usaspending-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/usaspending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/usaspending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### USAspending Subawards API

Paged, sortable listing of subawards (pass-through awards from a prime recipient to a subrecipient) scoped to a given prime award ID - subaward number, description, action date, amount, and subrecipient name. Powers the Sub-Awards tab on the USAspending.gov award profile page.

- **Human URL:** [https://api.usaspending.gov/docs/endpoints](https://api.usaspending.gov/docs/endpoints)
- **Base URL:** `https://api.usaspending.gov/api/v2`

#### Properties

- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [API Reference](https://github.com/fedspendingtransparency/usaspending-api/blob/master/usaspending_api/api_contracts/contracts/v2/subawards.md)
- [OpenAPI](openapi/usaspending-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/usaspending.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/usaspending.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/fedspendingtransparency)
- [Website](https://www.usaspending.gov)
- [Documentation](https://api.usaspending.gov/docs/endpoints)
- [Rate Limits](rate-limits/usaspending-rate-limits.yml)

## Pricing & FinOps

USAspending is free, public, open government data funded under the DATA Act - there is no account, no API key, no pricing tier, and no billing surface. This catalog entry intentionally has no `plans/` or `finops/` directory rather than fabricating pricing information that does not exist.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
