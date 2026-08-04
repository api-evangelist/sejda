# Sejda (sejda)

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

Sejda provides online and desktop tools for editing and manipulating PDF documents - merge, split, compress, convert, edit, watermark, OCR, and fill forms. Its only documented hosted REST API is the HTML-to-PDF conversion API at api.sejda.com; the broader merge/split/OCR task set is delivered through the web and desktop apps and through the open-source Sejda SDK and sejda-console (Java, AGPLv3), not a hosted task API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sejda/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sejda/refs/heads/main/apis.yml)

## Tags

- PDF
- Document Conversion
- HTML to PDF
- PDF Editing
- OCR

## Timestamps

- **Created:** 2026-06-25
- **Modified:** 2026-06-25

## APIs

### Sejda HTML to PDF API

The only documented Sejda hosted REST API. Converts a URL or raw HTML to a PDF document via POST https://api.sejda.com/v2/html-pdf with a JSON body, authenticated with a Token (or publishable) API key. Sejda explicitly states it does not offer hosted API access to its other PDF tools (e.g. merge, compress).

- **Human URL:** [https://www.sejda.com/developers](https://www.sejda.com/developers)
- **Base URL:** `https://api.sejda.com/v2`

#### Tags

- HTML to PDF
- Conversion
- REST

#### Properties

- [Documentation](https://www.sejda.com/developers)
- [Documentation](https://www.sejda.com/html-pdf-api)
- [OpenAPI](openapi/sejda-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sejda.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sejda.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sejda PDF Tools (Web and Desktop)

Sejda's full PDF task catalog - merge, split, compress, convert (Office/HTML to PDF, PDF to images), edit, watermark, OCR, and fill forms - delivered as online (browser) and desktop applications. These tasks are NOT exposed as a hosted REST API; only HTML-to-PDF has a documented API.

- **Human URL:** [https://www.sejda.com/](https://www.sejda.com/)

#### Tags

- PDF Editing
- Merge
- Split
- Compress
- Watermark
- OCR

#### Properties

- [Documentation](https://www.sejda.com/)
- [Documentation](https://www.sejda.com/help)

### Sejda SDK

Open-source (AGPLv3) Java library for PDF manipulation - merge, split, rotate, encrypt, watermark, and more - built on SAMBox (a maintained PDFBox fork). This is an embeddable code library, not a hosted network API; a commercial Pro license is available for non-AGPL use.

- **Human URL:** [https://sejda.org/](https://sejda.org/)

#### Tags

- SDK
- Java
- Open Source
- PDF Manipulation

#### Properties

- [Documentation](https://sejda.org/)
- [Source Code](https://github.com/torakiki/sejda)
- [Documentation](https://github.com/torakiki/sejda/wiki)

### Sejda Console

Command-line shell over the Sejda SDK for running PDF tasks (merge, split, etc.) from a terminal or scripts. Requires a Java runtime. A commercial sejda-console-pro build exists. This is a local CLI tool, not a hosted API.

- **Human URL:** [https://sejda.org/download](https://sejda.org/download)

#### Tags

- CLI
- Java
- Open Source
- PDF Manipulation

#### Properties

- [Documentation](https://sejda.org/download)
- [Documentation](https://github.com/torakiki/sejda/wiki)
- [Source Code](https://github.com/torakiki/sejda)

## Common Properties

- [GitHub Organization](https://github.com/sejda-pdf)
- [LinkedIn](https://www.linkedin.com/company/sejda)
- [Website](https://www.sejda.com)
- [Documentation](https://www.sejda.com/developers)
- [Plans](plans/sejda-plans-pricing.yml)
- [Rate Limits](rate-limits/sejda-rate-limits.yml)
- [Fin Ops](finops/sejda-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
