# APRA (apra)

The Australian Prudential Regulation Authority (APRA) is the Commonwealth statutory authority that prudentially supervises Australia's banks, credit unions, building societies, general insurers, life insurers, private health insurers, reinsurers and most of the superannuation industry, protecting depositors, policyholders and fund members under the Financial Sector (Collection of Data) Act 2001 and the Insurance Act 1973. Across insurance it authorises and registers general insurers, life insurers and friendly societies, and private health insurers; publishes prudential standards and practice guides; maintains public registers of authorised institutions; and runs the quarterly general, life and private health insurance performance statistics plus the National Claims and Policies Database.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/apra/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/apra/refs/heads/main/apis.yml)

## Tags

- Insurance
- Australia
- Regulator
- Prudential Regulation
- General Insurance
- Life Insurance
- Private Health Insurance
- Regulatory Reporting
- Market Infrastructure
- Risk Data
- Superannuation
- Banking

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

APRA publishes **no public API**. As of 25 July 2026 there is no developer portal, no OpenAPI or Swagger definition, no API key or OAuth scheme, no webhooks or AsyncAPI, no public Postman collection, and no GraphQL endpoint. Every conventional developer host was probed and none resolves — `developer.apra.gov.au`, `developers.apra.gov.au`, `docs.apra.gov.au` and `api.apra.gov.au` all fail DNS, and `/developers`, `/api`, `/developer`, `/partners` and `/integrations` on `apra.gov.au` all return HTTP 404.

The only integration surface is **APRA Connect**, the regulatory data-lodgement portal at [connect.apra.gov.au](https://connect.apra.gov.au), a browser application gated behind the Australian Government Digital ID System (myID for identity plus Relationship Authorisation Manager for the entity relationship). APRA's own [information security and technical specifications](https://www.apra.gov.au/apra-portals/apra-connect/apra-connect-information-security-and-technical-specifications) page settles it: the API Technical Specification is listed as *"to be provided when this functionality is available."* RegTech providers can request the [test environment](https://www.apra.gov.au/apra-portals/apra-connect/regtech-access-apra-connect-test) by signed deed — but that grants portal access, not API access.

What APRA does publish machine-readably is a **standards corpus, not an API**: the [APRA Connect taxonomy artefacts](https://www.apra.gov.au/apra-portals/apra-connect/apra-connect-taxonomy-artefacts) — XSD schemas explicitly intended for third-party software integration, reporting taxonomy workbooks, and validation rule spreadsheets — published per industry, including General Insurance (May 2026), Private Health Insurance (February 2026) and Life Insurance (February 2026). Accepted submission formats are manual entry, XML, XBRL and Excel.

**ACORD posture:** no ACORD reference found. A site search of apra.gov.au for ACORD returns nothing, and neither AL3, ACORD XML nor NGDS appears in any prudential standard, taxonomy artefact or statistical publication. APRA reports against its own XBRL/XSD data model rather than the insurance industry's ACORD messaging standards — expected for a prudential supervisor collecting solvency, capital and performance returns rather than policy and claims transactions.

**Quote / bind / issue / FNOL:** none, and none expected. APRA is a supervisor, not a carrier, broker or MGA.

## Market context

Australia has the legal machinery for open insurance and no live obligation. The Consumer Data Right opened banking and energy and was designated to extend to general insurance, then deferred and de-prioritised — so the CDR seam that made Australian banking legible stops before insurance. APRA is a prudential supervisor rather than a CDR data-standards body, and nothing pushes it toward a public API. Contrast the UK, where the FCA Financial Services Register API is real and documented; APRA's equivalent registers are HTML tables with no bulk export.

## Registers and data

- [Registers index](https://www.apra.gov.au/registers) — HTML only, no CSV/JSON/API export
- [List of general insurers](https://www.apra.gov.au/registers/list-general-insurance)
- [List of registered life insurers and friendly societies](https://www.apra.gov.au/registers/list-registered-life-insurers-and-friendly-societies)
- [List of registered private health insurers](https://www.apra.gov.au/registers/list-registered-private-health-insurers)
- [Statistical publications](https://www.apra.gov.au/statistics) — XLSX downloads plus Power BI dashboards
- [Quarterly general insurance performance statistics](https://www.apra.gov.au/news-and-publications/quarterly-general-insurance-performance-statistics)
- [Quarterly life insurance performance statistics](https://www.apra.gov.au/news-and-publications/quarterly-life-insurance-performance-statistics)
- [Quarterly private health insurance performance statistics](https://www.apra.gov.au/news-and-publications/quarterly-private-health-insurance-performance-statistics)
- [National Claims and Policies Database statistics](https://www.apra.gov.au/news-and-publications/national-claims-and-policies-database-statistics)

APRA has no publisher presence on data.gov.au — a CKAN query for an APRA organisation returned zero datasets.

## Links

- **Website:** [https://www.apra.gov.au/](https://www.apra.gov.au/)
- **News and publications:** [https://www.apra.gov.au/news-and-publications](https://www.apra.gov.au/news-and-publications)
- **RSS:** [https://www.apra.gov.au/rss.xml](https://www.apra.gov.au/rss.xml)
- **Prudential standards and guidance:** [https://www.apra.gov.au/prudential-standards-and-guidance](https://www.apra.gov.au/prudential-standards-and-guidance)
- **APRA Connect:** [https://www.apra.gov.au/apra-portals/apra-connect](https://www.apra.gov.au/apra-portals/apra-connect)
- **LinkedIn:** [https://www.linkedin.com/company/apra](https://www.linkedin.com/company/apra)
- **Data enquiries:** dataanalytics@apra.gov.au
