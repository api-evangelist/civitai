# Civitai

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

Civitai is the largest open community for Stable Diffusion, SDXL, Flux, and video AI models — hosting over a million model checkpoints, LoRAs, embeddings, and VAEs uploaded and rated by creators. Beyond hosting, Civitai operates a hosted AI image, video, audio, and language generation service through its Orchestration API, which races workflows across providers (Flux 1/2, SDXL, SD1, Z-Image, Qwen, Seedream, Grok, WAN 2.1-2.7, Kling, LTX2, Vidu, Veo 3, HunyuanVideo) and supports LoRA training jobs. The Site API exposes the public catalog plus user vault, permissions, and AIR identifier resolution. OAuth 2.0 with PKCE and per-app Buzz spend caps lets third parties build delegated experiences without owning a user's full credit balance. Generation is metered in Buzz, a virtual credit topped up via memberships or one-off packs.

**Areas:** Artificial Intelligence · Image Generation · Video Generation · Stable Diffusion · SDXL · Flux · LoRA · Model Hosting · Community · Generative AI

## Civitai on APIs.io

Everything profiled for Civitai is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/civitai/](https://apis.io/providers/civitai/)** — or go straight to one of the APIs or properties below.

### APIs (12)

- [Civitai OAuth API](https://apis.io/apis/civitai/civitai-oauth-api/) — OAuth 2.0 authorization-code with PKCE for third-party apps that act on behalf of a Civitai user. Supports scoped tokens, refresh flow, and per-app Buzz…
- [Civitai Blobs API](https://apis.io/apis/civitai/civitai-blobs-api/) — Upload and reference blobs for inputs and outputs.
- [Civitai Creators API](https://apis.io/apis/civitai/civitai-creators-api/) — Users who publish models.
- [Civitai Enums API](https://apis.io/apis/civitai/civitai-enums-api/) — Enumerations used throughout the API.
- [Civitai Images API](https://apis.io/apis/civitai/civitai-images-api/) — Community-shared generation outputs.
- [Civitai Models API](https://apis.io/apis/civitai/civitai-models-api/) — Catalog of model checkpoints, LoRAs, embeddings, and VAEs.
- [Civitai Permissions API](https://apis.io/apis/civitai/civitai-permissions-api/) — Permission checks for the current bearer.
- [Civitai Tags API](https://apis.io/apis/civitai/civitai-tags-api/) — Catalog tag taxonomy.
- [Civitai Users API](https://apis.io/apis/civitai/civitai-users-api/) — User accounts.
- [Civitai Vault API](https://apis.io/apis/civitai/civitai-vault-api/) — A user's saved-model vault (membership tiers).
- [Civitai Workflows API](https://apis.io/apis/civitai/civitai-workflows-api/) — Submit and manage generation workflows.
- [Civitai Model Versions API](https://apis.io/apis/civitai/civitai-model-versions-api/) — Specific versions of a model with files, hashes, and AIR identifiers.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (13)

Multi-step workflows that chain operations into a business task.

- [Civitai Batch Hash Reconciliation](https://apis.io/arazzos/civitai/civitai-batch-hash-reconcile-workflow/)
- [Civitai Blob Upload and Image-to-Image Generation](https://apis.io/arazzos/civitai/civitai-blob-upload-img2img-workflow/)
- [Civitai Creator Models and Image Gallery](https://apis.io/arazzos/civitai/civitai-creator-models-gallery-workflow/)
- [Civitai Image Generation Submit and Poll](https://apis.io/arazzos/civitai/civitai-image-generation-poll-workflow/)
- [Civitai Model Images Explorer](https://apis.io/arazzos/civitai/civitai-model-images-explorer-workflow/)
- [Civitai Identify a Model From a File Hash](https://apis.io/arazzos/civitai/civitai-model-version-by-hash-workflow/)
- [Civitai Generate From a Catalog Model Version](https://apis.io/arazzos/civitai/civitai-model-version-to-generation-workflow/)
- [Civitai Permission-Gated Version Download](https://apis.io/arazzos/civitai/civitai-permission-gated-download-workflow/)
- [Civitai Presigned Blob Upload Then Generate](https://apis.io/arazzos/civitai/civitai-presigned-blob-generate-workflow/)
- [Civitai Search Models and Drill Into a Version](https://apis.io/arazzos/civitai/civitai-search-models-detail-workflow/)
- [Civitai Tag-Driven Model Discovery](https://apis.io/arazzos/civitai/civitai-tag-models-discovery-workflow/)
- [Civitai Vault Add and Verify](https://apis.io/arazzos/civitai/civitai-vault-toggle-verify-workflow/)
- [Civitai Query and Cancel a Running Workflow](https://apis.io/arazzos/civitai/civitai-workflow-query-cancel-workflow/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Civitai MCP Server](https://apis.io/servers/civitai/civitai-mcp-server/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Civitai Agentic Access](https://apis.io/agentic-access/civitai/civitai-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Civitai Image](https://apis.io/schemas/civitai/civitai-image/)
- [Civitai Model](https://apis.io/schemas/civitai/civitai-model/)
- [Civitai Orchestration Workflow](https://apis.io/schemas/civitai/civitai-workflow/)

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Civitai Model Structure](https://apis.io/json-structure/civitai/civitai-model-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Civitai Context](https://apis.io/jsonld/civitai/civitai-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Civitai Vocabulary](https://apis.io/vocabularies/civitai/civitai-vocabulary/)

#### Examples (2)

Example requests and responses.

- [Civitai Image Generation Example](https://apis.io/examples/civitai/civitai-image-generation-example/)
- [Civitai Video Generation Example](https://apis.io/examples/civitai/civitai-video-generation-example/)

#### Collections (15)

Postman and Open Collection request collections.

- [Civitai Orchestration Blobs API](https://apis.io/collections/civitai/open-civitai-blobs-api/)
- [Civitai Orchestration Blobs Creators API](https://apis.io/collections/civitai/open-civitai-creators-api/)
- [Civitai Orchestration Blobs Enums API](https://apis.io/collections/civitai/open-civitai-enums-api/)
- [Civitai Orchestration Blobs Images API](https://apis.io/collections/civitai/open-civitai-images-api/)
- [Civitai Orchestration Blobs Models API](https://apis.io/collections/civitai/open-civitai-models-api/)
- [Civitai Orchestration Blobs ModelVersions API](https://apis.io/collections/civitai/open-civitai-modelversions-api/)
- [Civitai Orchestration API](https://apis.io/collections/civitai/open-civitai-orchestration-api/)
- [Civitai Orchestration Blobs Permissions API](https://apis.io/collections/civitai/open-civitai-permissions-api/)
- [Civitai Site API](https://apis.io/collections/civitai/open-civitai-site-api/)
- [Civitai Orchestration Blobs Tags API](https://apis.io/collections/civitai/open-civitai-tags-api/)
- [Civitai Orchestration Blobs Users API](https://apis.io/collections/civitai/open-civitai-users-api/)
- [Civitai Orchestration Blobs Vault API](https://apis.io/collections/civitai/open-civitai-vault-api/)
- [Civitai Orchestration Blobs Workflows API](https://apis.io/collections/civitai/open-civitai-workflows-api/)
- [Civitai Orchestration API](https://apis.io/collections/civitai/postman-civitai-orchestration-api/)
- [Civitai Site API](https://apis.io/collections/civitai/postman-civitai-site-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Civitai — jsonschema rules](https://apis.io/rules/civitai/civitai-jsonschema-spectral-rules/)
- [Civitai API Rules](https://apis.io/rules/civitai/civitai-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Civitai Authentication](https://apis.io/security/civitai/civitai-authentication/)
- [Civitai Domain Security](https://apis.io/security/civitai/civitai-domain-security/)
- [Civitai Vulnerability Disclosure](https://apis.io/security/civitai/civitai-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Civitai Plans Pricing](https://apis.io/plans/civitai/civitai-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Civitai Rate Limits](https://apis.io/rate-limits/civitai/civitai-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Civitai Finops](https://apis.io/finops/civitai/civitai-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.civitai.com/)
- [Documentation](https://developer.civitai.com/)
- [Getting started](https://developer.civitai.com/orchestration/guide/getting-started)
- [Support](https://education.civitai.com/)
- [Blog](https://civitai.com/articles)
- [Terms of service](https://civitai.com/content/tos)
- [Privacy policy](https://civitai.com/content/privacy)
- [GitHub](https://github.com/civitai)

## API Evangelist rating

**Kin Score 49.7** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 56.7 |
| Contract quality | 64.4 |
| Contract governance | 13.6 |
| Operational transparency | 28.9 |
| Developer ergonomics | 58.3 |
| Access clarity | 50.0 |

**Agent readiness 31.2** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | unknown |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 28.2** — AI & Biometrics

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/civitai/](https://apis.io/providers/civitai/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Civitai: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/civitai/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
