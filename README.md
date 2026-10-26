# PDFEndpoint (pdfendpoint)

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

PDFEndpoint is a lightweight HTML and URL to PDF conversion API. A single REST endpoint renders raw HTML or a publicly accessible HTTPS URL into a PDF using a headless browser, with extensive options for page size, margins, orientation, headers and footers, encryption, and multiple delivery modes (JSON URL, base64, inline, webhook, S3, GCP). A sandbox mode watermarks output without consuming the monthly quota.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/pdfendpoint/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/pdfendpoint/refs/heads/main/apis.yml)

## Tags

- PDF
- HTML to PDF
- URL to PDF
- Document Generation
- Conversion

## Timestamps

- **Created:** 2026-06-25
- **Modified:** 2026-06-25

## APIs

### PDFEndpoint Convert HTML API

Converts raw HTML content into a PDF via POST /convert, with options for page size, orientation, margins, viewport, zoom, CSS/JS injection, Liquid templating, headers and footers, image compression, and encryption.

- **Human URL:** [https://pdfendpoint.com/docs](https://pdfendpoint.com/docs)
- **Base URL:** `https://api.pdfendpoint.com/v1`

#### Tags

- PDF
- HTML to PDF
- Conversion

#### Properties

- [Documentation](https://pdfendpoint.com/docs)
- [OpenAPI](openapi/pdfendpoint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pdfendpoint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pdfendpoint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PDFEndpoint Convert URL API

Converts a publicly accessible HTTPS URL into a PDF via POST /convert using the url parameter, with wait-for-selector, network, cookie, header, basic auth, and geolocation controls for rendering dynamic pages.

- **Human URL:** [https://pdfendpoint.com/docs/document/url](https://pdfendpoint.com/docs/document/url)
- **Base URL:** `https://api.pdfendpoint.com/v1`

#### Tags

- PDF
- URL to PDF
- Conversion

#### Properties

- [Documentation](https://pdfendpoint.com/docs/document/url)
- [OpenAPI](openapi/pdfendpoint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pdfendpoint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pdfendpoint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PDFEndpoint Renders and Delivery API

Manages generated renders and delivery. Supports delivery modes including json, base64, inline, webhook, s3, gcp, and jsonp; lists created PDFs via GET /list, deletes a render via DELETE /remove/{task_id}, and reports usage via GET /usage and health via GET /health.

- **Human URL:** [https://pdfendpoint.com/docs/delivery-mode](https://pdfendpoint.com/docs/delivery-mode)
- **Base URL:** `https://api.pdfendpoint.com/v1`

#### Tags

- PDF
- Webhooks
- Storage

#### Properties

- [Documentation](https://pdfendpoint.com/docs/delivery-mode)
- [OpenAPI](openapi/pdfendpoint-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pdfendpoint.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pdfendpoint.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://pdfendpoint.com)
- [Documentation](https://pdfendpoint.com/docs)
- [Plans](plans/pdfendpoint-plans-pricing.yml)
- [Rate Limits](rate-limits/pdfendpoint-rate-limits.yml)
- [Fin Ops](finops/pdfendpoint-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
