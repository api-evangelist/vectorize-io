# Vectorize (vectorize-io)

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
