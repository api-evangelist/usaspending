# USAspending.gov (usaspending)

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
