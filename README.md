# Civitai (civitai)

Civitai is the largest open community for Stable Diffusion, SDXL, Flux, and video AI models — hosting over a million model checkpoints, LoRAs, embeddings, and VAEs uploaded and rated by creators. Beyond hosting, Civitai operates a hosted AI image, video, audio, and language generation service through its Orchestration API, which races workflows across providers (Flux 1/2, SDXL, SD1, Z-Image, Qwen, Seedream, Grok, WAN 2.1-2.7, Kling, LTX2, Vidu, Veo 3, HunyuanVideo) and supports LoRA training jobs. The Site API exposes the public catalog plus user vault, permissions, and AIR identifier resolution. OAuth 2.0 with PKCE and per-app Buzz spend caps lets third parties build delegated experiences without owning a user's full credit balance. Generation is metered in Buzz, a virtual credit topped up via memberships or one-off packs.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/civitai/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- AI, Artificial Intelligence, Image Generation, Video Generation, Stable Diffusion, SDXL, Flux, LoRA, Model Hosting, Community, Generative AI

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Surfaces

| Surface | Base URL | Purpose |
|---|---|---|
| Site API | `https://civitai.com/api/v1/` | Browse the public model and image catalog; manage Vault and permissions. |
| Orchestration API | `https://orchestration.civitai.com` | Submit AI generation workflows (image, video, audio, language, training). |
| OAuth API | `https://civitai.com/api/oauth/...` | Authorization-code with PKCE for third-party apps acting on a user's behalf. |

## Engines available via Orchestration

| Modality | Engines |
|---|---|
| Image | Flux 2 (Klein / Dev / Flex / Pro / Max), Flux 1, SDXL, SD1, Z-Image, Qwen, Seedream, Grok |
| Video | WAN 2.1-2.7, Kling, LTX2, Vidu 2.0 / Q3, Veo 3 (standard/fast/lite), HunyuanVideo |
| Audio | Qwen3-ASR transcription, TTS with voice cloning, multi-speaker dialogue, ACE-Step music |
| Language | Chat completion via OpenRouter/AIR models with vision and tool support |
| Training | LoRA training for SDXL, Flux, WAN, and LTX2 ecosystems |
| Utilities | FlashVSR video upscaling, VFIMamba frame interpolation, ESRGAN image upscaling |

## APIs

### Civitai Site API
Browse and search the Civitai public catalog of Stable Diffusion, SDXL, Flux, and video models. Exposes models, model versions, images, creators, tags, users, permissions, and the user vault. Public read endpoints are cached; authenticated endpoints are not. Authenticate with a personal API key issued at civitai.com using a Bearer token.

**Human URL:** [https://developer.civitai.com/site/reference/](https://developer.civitai.com/site/reference/)

- [Documentation — Site Guide](https://developer.civitai.com/site/)
- [Documentation — Reference](https://developer.civitai.com/site/reference/)
- [OpenAPI](openapi/civitai-site-api-openapi.yml)
- [JSON Schema — Model](json-schema/civitai-model-schema.json)
- [JSON Schema — Image](json-schema/civitai-image-schema.json)
- [JSON-LD](json-ld/civitai-context.jsonld)
- [Naftiko Capability — Models](capabilities/site-models.yaml)
- [Naftiko Capability — Images](capabilities/site-images.yaml)
- [Naftiko Capability — Creators / Tags](capabilities/site-creators.yaml)
- [Naftiko Capability — Users](capabilities/site-users.yaml)
- [Naftiko Capability — Vault](capabilities/site-vault.yaml)
- [Naftiko Capability — Permissions](capabilities/site-permissions.yaml)

### Civitai Orchestration API
Submit AI generation workflows — image, video, audio, language, and LoRA training — through a single contract at `https://orchestration.civitai.com`. Races multiple providers and engines behind one workflow API. Includes blob upload with NSFW moderation, presigned URLs, in-order serialized webhooks (`workflow:succeeded`, `workflow:failed`, etc.), and Buzz-metered billing. Bearer-token authenticated.

**Human URL:** [https://developer.civitai.com/orchestration/reference/](https://developer.civitai.com/orchestration/reference/)

- [Documentation — Orchestration Guide](https://developer.civitai.com/orchestration/guide/)
- [Documentation — Recipes](https://developer.civitai.com/orchestration/recipes/)
- [Documentation — Webhooks](https://developer.civitai.com/orchestration/guide/results-and-webhooks)
- [Documentation — Authentication](https://developer.civitai.com/orchestration/guide/authentication)
- [OpenAPI](openapi/civitai-orchestration-api-openapi.yml)
- [JSON Schema — Workflow](json-schema/civitai-workflow-schema.json)
- [Example — Image Generation](examples/civitai-image-generation-example.json)
- [Example — Video Generation](examples/civitai-video-generation-example.json)
- [Naftiko Capability — Workflows](capabilities/orchestration-workflows.yaml)
- [Naftiko Capability — Blobs](capabilities/orchestration-blobs.yaml)
- [Naftiko Capability — Image Generation](capabilities/orchestration-image-generation.yaml)
- [Naftiko Capability — Video Generation](capabilities/orchestration-video-generation.yaml)
- [Naftiko Capability — Audio](capabilities/orchestration-audio.yaml)
- [Naftiko Capability — Training](capabilities/orchestration-training.yaml)

### Civitai OAuth API
OAuth 2.0 authorization-code with PKCE for third-party apps that act on behalf of a Civitai user. Supports scoped tokens, refresh flow, and per-app Buzz spend caps so a delegated app cannot drain a user's credit balance. Used by `civitai-app-starters` and `civitai-client-javascript` SDKs for building partner integrations against the Site and Orchestration APIs.

**Human URL:** [https://developer.civitai.com/site/oauth/](https://developer.civitai.com/site/oauth/)

- [Documentation — OAuth Overview](https://developer.civitai.com/site/oauth/)
- [Documentation — Register App](https://developer.civitai.com/site/oauth/register-app)
- [Documentation — Scopes](https://developer.civitai.com/site/oauth/scopes)
- [Documentation — Buzz Limits](https://developer.civitai.com/site/oauth/buzz-limits)
- [Naftiko Capability — OAuth](capabilities/oauth-authorization.yaml)

## Common Properties

- [Portal — civitai.com](https://civitai.com)
- [Documentation — developer.civitai.com](https://developer.civitai.com/)
- [Documentation — education.civitai.com](https://education.civitai.com/)
- [GettingStarted](https://developer.civitai.com/orchestration/guide/getting-started)
- [Authentication](https://developer.civitai.com/orchestration/guide/authentication)
- [Webhooks](https://developer.civitai.com/orchestration/guide/results-and-webhooks)
- [Errors](https://developer.civitai.com/orchestration/guide/errors-and-retries)
- [GitHubOrganization](https://github.com/civitai)
- [LinkedIn](https://www.linkedin.com/company/civitai)
- [Twitter](https://twitter.com/HelloCivitai)
- [SignUp](https://civitai.com/login)
- [TermsOfService](https://civitai.com/content/tos)
- [PrivacyPolicy](https://civitai.com/content/privacy)
- [ContentPolicy](https://civitai.com/content/content-policy)
- [Blog](https://civitai.com/articles)
- [Forum](https://education.civitai.com/forums/)
- [Support](https://education.civitai.com/)
- [SDK — JavaScript Client](https://github.com/civitai/civitai-client-javascript)
- [SDK — App Starters (OAuth + PKCE)](https://github.com/civitai/civitai-app-starters)
- [Tool — Civitai Link Desktop](https://github.com/civitai/civitai-link-desktop)
- [Tool — AI Toolkit](https://github.com/civitai/ai-toolkit)
- [Tool — Model Scanner](https://github.com/civitai/model-scanner)
- [Tool — ComfyUI fork](https://github.com/civitai/ComfyUI)
- [Plugins — ComfyUI smZNodes](https://github.com/civitai/ComfyUI_smZNodes)
- [GitHubRepository — Civitai Platform](https://github.com/civitai/civitai)
- [Documentation — AIR (AI Resource Identifier)](https://developer.civitai.com/site/guide/air)
- [MCPServer — Civitai MCP](https://developer.civitai.com/orchestration/mcp)
- [Documentation — llms.txt](https://developer.civitai.com/llms.txt)
- [Documentation — llms-full.txt](https://developer.civitai.com/llms-full.txt)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Civitai Site API](openapi/civitai-site-api-openapi.yml)
- [Civitai Orchestration API](openapi/civitai-orchestration-api-openapi.yml)

### JSON Schema

- [Civitai Model](json-schema/civitai-model-schema.json)
- [Civitai Image](json-schema/civitai-image-schema.json)
- [Civitai Workflow](json-schema/civitai-workflow-schema.json)

### JSON Structure

- [Civitai Model Structure](json-structure/civitai-model-structure.json)

### JSON-LD

- [Civitai Context](json-ld/civitai-context.jsonld)

### Examples

- [Image Generation (SDXL)](examples/civitai-image-generation-example.json)
- [Video Generation (WAN 2.5)](examples/civitai-video-generation-example.json)

### Vocabulary

- [Civitai Vocabulary](vocabulary/civitai-vocabulary.yml)

### Capabilities (Naftiko)

- [Site — Models](capabilities/site-models.yaml)
- [Site — Images](capabilities/site-images.yaml)
- [Site — Creators / Tags](capabilities/site-creators.yaml)
- [Site — Users](capabilities/site-users.yaml)
- [Site — Vault](capabilities/site-vault.yaml)
- [Site — Permissions](capabilities/site-permissions.yaml)
- [Orchestration — Workflows](capabilities/orchestration-workflows.yaml)
- [Orchestration — Blobs](capabilities/orchestration-blobs.yaml)
- [Orchestration — Image Generation](capabilities/orchestration-image-generation.yaml)
- [Orchestration — Video Generation](capabilities/orchestration-video-generation.yaml)
- [Orchestration — Audio](capabilities/orchestration-audio.yaml)
- [Orchestration — LoRA Training](capabilities/orchestration-training.yaml)
- [OAuth — Authorization](capabilities/oauth-authorization.yaml)

### Spectral Rules

- [Civitai Rules](rules/civitai-rules.yml)

### Commercial Artifacts

- [Plans / Pricing](plans/civitai-plans-pricing.yml)
- [Rate Limits](rate-limits/civitai-rate-limits.yml)
- [FinOps Definition](finops/civitai-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
