# APRA (apra)

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
