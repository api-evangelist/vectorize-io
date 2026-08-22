# Vectorize (vectorize-io)

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

Vectorize is a RAG (retrieval-augmented generation) pipeline platform that ingests unstructured data, chunks and embeds it, and serves low-latency retrieval against a managed vector database. The Vectorize API lets developers create, start, and stop RAG pipelines, run retrieval, manage source / destination / AI-platform connectors, upload files, extract documents with Iris, and run deep research.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/apis.yml)

## Tags

- AI
- RAG
- Vectorization
- Embeddings
- Retrieval
- Vector Database

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Vectorize Pipelines API

Create, list, retrieve, start, stop, and delete organization-scoped RAG pipelines that wire source connectors, an AI-platform embedding connector, and a destination vector database together, plus pipeline events and metrics.

- **Human URL:** [https://docs.vectorize.io/reference/api/api-getting-started/](https://docs.vectorize.io/reference/api/api-getting-started/)
- **Base URL:** `https://api.vectorize.io/v1`

#### Tags

- RAG
- Pipelines
- Ingest

#### Properties

- [Documentation](https://docs.vectorize.io/build-deploy/data-pipelines/)
- [API Reference](https://docs.vectorize.io/reference/api/api-getting-started/)
- [OpenAPI](openapi/vectorize-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vectorize-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vectorize-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vectorize Retrieval API

Per-pipeline retrieval endpoint that vectorizes the input question, runs a k-ANN search against the pipeline's vector index, applies optional reranking and metadata filters, and returns ranked document chunks with relevancy scores.

- **Human URL:** [https://docs.vectorize.io/build-deploy/data-pipelines/retrieval-endpoint/](https://docs.vectorize.io/build-deploy/data-pipelines/retrieval-endpoint/)
- **Base URL:** `https://api.vectorize.io/v1`

#### Tags

- Retrieval
- Search
- Reranking

#### Properties

- [Documentation](https://docs.vectorize.io/build-deploy/data-pipelines/retrieval-endpoint/)
- [API Reference](https://docs.vectorize.io/reference/api/api-getting-started/)
- [OpenAPI](openapi/vectorize-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vectorize-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vectorize-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vectorize Connectors API

CRUD management of source connectors (data sources), destination connectors (vector databases), and AI-platform connectors (embedding / model providers), plus per-source user authorization for OAuth-style connectors.

- **Human URL:** [https://docs.vectorize.io/reference/api/api-getting-started/](https://docs.vectorize.io/reference/api/api-getting-started/)
- **Base URL:** `https://api.vectorize.io/v1`

#### Tags

- Connectors
- Sources
- Destinations

#### Properties

- [Documentation](https://docs.vectorize.io/integrations/)
- [API Reference](https://docs.vectorize.io/reference/api/api-getting-started/)
- [OpenAPI](openapi/vectorize-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vectorize-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vectorize-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vectorize File Upload API

Upload generic files to the platform via a pre-signed URL flow, and push or delete files against a File Upload source connector for ingestion into a pipeline.

- **Human URL:** [https://docs.vectorize.io/reference/api/api-getting-started/](https://docs.vectorize.io/reference/api/api-getting-started/)
- **Base URL:** `https://api.vectorize.io/v1`

#### Tags

- Files
- Upload
- Storage

#### Properties

- [Documentation](https://docs.vectorize.io/build-deploy/data-sources/)
- [API Reference](https://docs.vectorize.io/reference/api/api-getting-started/)
- [OpenAPI](openapi/vectorize-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vectorize-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vectorize-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vectorize Extraction (Iris) API

Vectorize Iris document extraction - start an extraction job against an uploaded file to convert it into Markdown chunks with optional metadata, and poll for the asynchronous extraction result.

- **Human URL:** [https://docs.vectorize.io/build-deploy/extract-information/understanding-iris/](https://docs.vectorize.io/build-deploy/extract-information/understanding-iris/)
- **Base URL:** `https://api.vectorize.io/v1`

#### Tags

- Extraction
- Iris
- Chunking

#### Properties

- [Documentation](https://docs.vectorize.io/build-deploy/extract-information/understanding-iris/)
- [API Reference](https://docs.vectorize.io/reference/api/api-getting-started/)
- [OpenAPI](openapi/vectorize-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vectorize-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vectorize-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vectorize Deep Research API

Start a private deep-research run grounded in a pipeline's vector index (optionally augmented with web search) and poll for the generated research report.

- **Human URL:** [https://docs.vectorize.io/reference/api/api-getting-started/](https://docs.vectorize.io/reference/api/api-getting-started/)
- **Base URL:** `https://api.vectorize.io/v1`

#### Tags

- Deep Research
- Agents
- RAG

#### Properties

- [Documentation](https://docs.vectorize.io/build-deploy/data-pipelines/)
- [API Reference](https://docs.vectorize.io/reference/api/api-getting-started/)
- [OpenAPI](openapi/vectorize-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vectorize-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vectorize-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/vectorize-io)
- [LinkedIn](https://www.linkedin.com/company/vectorize-io)
- [Website](https://vectorize.io/)
- [Documentation](https://docs.vectorize.io)
- [Plans](plans/vectorize-io-plans-pricing.yml)
- [Rate Limits](rate-limits/vectorize-io-rate-limits.yml)
- [Fin Ops](finops/vectorize-io-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
