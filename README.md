# Civitai (civitai)

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

Civitai is the largest open community for Stable Diffusion, SDXL, Flux, and video AI models — hosting over a million model checkpoints, LoRAs, embeddings, and VAEs uploaded and rated by creators. Beyond hosting, Civitai operates a hosted AI image, video, audio, and language generation service through its Orchestration API, which races workflows across providers (Flux 1/2, SDXL, SD1, Z-Image, Qwen, Seedream, Grok, WAN 2.1-2.7, Kling, LTX2, Vidu, Veo 3, HunyuanVideo) and supports LoRA training jobs. The Site API exposes the public catalog plus user vault, permissions, and AIR identifier resolution. OAuth 2.0 with PKCE and per-app Buzz spend caps lets third parties build delegated experiences without owning a user's full credit balance. Generation is metered in Buzz, a virtual credit topped up via memberships or one-off packs.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/apis.yml)

## Scope

- **Position:** Producing
- **Access:** 3rd-Party

## Tags

- AI
- Artificial Intelligence
- Image Generation
- Video Generation
- Stable Diffusion
- SDXL
- Flux
- LoRA
- Model Hosting
- Community
- Generative AI

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Civitai Site API

Browse and search the Civitai public catalog of Stable Diffusion, SDXL, Flux, and video models. The Site API exposes models, model versions, images, creators, tags, users, permissions, and the user vault over `https://civitai.com/api/v1/`. Supports hash-based version lookup, AIR identifiers, and Bearer-token authentication via personal API keys. Public endpoints are cached; authenticated endpoints are not.

- **Human URL:** [https://developer.civitai.com/site/reference/](https://developer.civitai.com/site/reference/)

#### Tags

- AI
- Artificial Intelligence
- Image Generation
- Models
- Stable Diffusion
- Flux
- LoRA
- Community

#### Properties

- [Documentation](https://developer.civitai.com/site/)
- [Documentation](https://developer.civitai.com/site/reference/)
- [Documentation](https://developer.civitai.com/site/reference/models)
- [Documentation](https://developer.civitai.com/site/reference/images)
- [Documentation](https://developer.civitai.com/site/reference/creators)
- [Documentation](https://developer.civitai.com/site/reference/users)
- [Documentation](https://developer.civitai.com/site/reference/permissions)
- [Documentation](https://developer.civitai.com/site/reference/vault)
- [OpenAPI](openapi/civitai-site-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/civitai-site-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/civitai-site-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/civitai-model-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/civitai-image-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/civitai-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Civitai Orchestration API

Submit AI generation workflows — image, video, audio, language, and LoRA training — through a single contract at `https://orchestration.civitai.com`. Races multiple providers and engines (Flux 1/2, SDXL, SD1, Z-Image, Qwen, Seedream, Grok, WAN 2.1-2.7, Kling, LTX2, Vidu, Veo 3, HunyuanVideo) behind one workflow API. Includes blob upload with NSFW moderation, presigned URLs, in-order serialized webhooks (`workflow:succeeded`, `workflow:failed`, etc.), and Buzz-metered billing. Bearer-token authenticated.

- **Human URL:** [https://developer.civitai.com/orchestration/reference/](https://developer.civitai.com/orchestration/reference/)

#### Tags

- AI
- Artificial Intelligence
- Image Generation
- Video Generation
- Audio Generation
- LoRA Training
- Webhooks
- Workflows

#### Properties

- [Documentation](https://developer.civitai.com/orchestration/)
- [Documentation](https://developer.civitai.com/orchestration/guide/)
- [Documentation](https://developer.civitai.com/orchestration/guide/getting-started)
- [Authentication](https://developer.civitai.com/orchestration/guide/authentication)
- [Documentation](https://developer.civitai.com/orchestration/guide/workflows)
- [Documentation](https://developer.civitai.com/orchestration/guide/submitting-work)
- [Webhooks](https://developer.civitai.com/orchestration/guide/results-and-webhooks)
- [Errors](https://developer.civitai.com/orchestration/guide/errors-and-retries)
- [Documentation](https://developer.civitai.com/orchestration/reference/)
- [Documentation](https://developer.civitai.com/orchestration/recipes/)
- [OpenAPI](openapi/civitai-orchestration-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/civitai-orchestration-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/civitai-orchestration-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/civitai-workflow-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/civitai-image-generation-example.json)
- [Example](examples/civitai-video-generation-example.json)

### Civitai OAuth API

OAuth 2.0 authorization-code with PKCE for third-party apps that act on behalf of a Civitai user. Supports scoped tokens, refresh flow, and per-app Buzz spend caps so a delegated app cannot drain a user's credit balance. Used by `civitai-app-starters` and `civitai-client-javascript` SDKs for building partner integrations against the Site and Orchestration APIs.

- **Human URL:** [https://developer.civitai.com/site/oauth/](https://developer.civitai.com/site/oauth/)

#### Tags

- AI
- Artificial Intelligence
- Authentication
- OAuth
- PKCE
- Identity

#### Properties

- [Documentation](https://developer.civitai.com/site/oauth/)
- [Documentation](https://developer.civitai.com/site/oauth/register-app)
- [Documentation](https://developer.civitai.com/site/oauth/scopes)
- [Documentation](https://developer.civitai.com/site/oauth/buzz-limits)
- [Postman Collection](collections/civitai-orchestration-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/civitai-orchestration-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/civitai-site-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/civitai-site-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [LinkedIn](https://www.linkedin.com/company/civitai)
- [Twitter](https://twitter.com/HelloCivitai)
- [GitHub Organization](https://github.com/civitai)
- [Portal](https://civitai.com)
- [Documentation](https://developer.civitai.com/)
- [Documentation](https://education.civitai.com/)
- [Getting Started](https://developer.civitai.com/orchestration/guide/getting-started)
- [Authentication](https://developer.civitai.com/orchestration/guide/authentication)
- [Webhooks](https://developer.civitai.com/orchestration/guide/results-and-webhooks)
- [Errors](https://developer.civitai.com/orchestration/guide/errors-and-retries)
- [Sign Up](https://civitai.com/login)
- [Terms of Service](https://civitai.com/content/tos)
- [Privacy Policy](https://civitai.com/content/privacy)
- [Content Policy](https://civitai.com/content/content-policy)
- [Support](https://education.civitai.com/)
- [Blog](https://civitai.com/articles)
- [Forum](https://education.civitai.com/forums/)
- [SDK](https://github.com/civitai/civitai-client-javascript)
- [SDK](https://github.com/civitai/civitai-app-starters)
- [Tool](https://github.com/civitai/civitai-link-desktop)
- [GitHub Repository](https://github.com/civitai/civitai)
- [Tool](https://github.com/civitai/ai-toolkit)
- [Tool](https://github.com/civitai/model-scanner)
- [Tool](https://github.com/civitai/ComfyUI)
- [Plugins](https://github.com/civitai/ComfyUI_smZNodes)
- [GitHub Repository](https://github.com/civitai/bitdex)
- [Documentation](https://developer.civitai.com/site/guide/air)
- [M C P Server](https://developer.civitai.com/orchestration/mcp)
- [Documentation](https://developer.civitai.com/llms.txt)
- [Documentation](https://developer.civitai.com/llms-full.txt)
- [Plans](plans/civitai-plans-pricing.yml)
- [Rate Limits](rate-limits/civitai-rate-limits.yml)
- [Fin Ops](finops/civitai-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
