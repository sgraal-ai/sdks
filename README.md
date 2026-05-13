<p align="center">
  <img src="./assets/sgraal_mark_adaptive.svg" alt="Sgraal" width="48" height="48">
</p>

# Sgraal SDKs

Official open-source SDKs for **Sgraal** — vendor-neutral memory governance layer for AI agents.

Each SDK wraps the public [`POST /v1/preflight`](https://sgraal.com/docs/api) endpoint and returns a four-band decision (`USE_MEMORY` / `WARN` / `ASK_USER` / `BLOCK`) so your agent can act on its memory only when the memory is reliable.

| SDK | Language | Install | Status | Source |
|---|---|---|---|---|
| **langchain-sgraal** | Python | `pip install langchain-sgraal` | Production | [`./langchain-sgraal/`](./langchain-sgraal/) |
| **mem0-sgraal** | Python | `pip install mem0-sgraal` | Production | [`./mem0-sgraal/`](./mem0-sgraal/) |
| **openai-sgraal** | Python | `pip install openai-sgraal` | Production | [`./openai-sgraal/`](./openai-sgraal/) |
| **crewai-sgraal** | Python | `pip install crewai-sgraal` | Production | [`./crewai-sgraal/`](./crewai-sgraal/) |
| **autogen-sgraal** | Python | `pip install autogen-sgraal` | Production | [`./autogen-sgraal/`](./autogen-sgraal/) |
| **sgraal-rag** | Python | `pip install sgraal-rag` | Production | [`./sgraal-rag/`](./sgraal-rag/) |
| **@sgraal/mcp** | TypeScript / Node | `npm install @sgraal/mcp` | Production | [`./mcp/`](./mcp/) |
| **llamaindex-sgraal** | Python | `pip install llamaindex-sgraal` | Beta | [`./llamaindex-sgraal/`](./llamaindex-sgraal/) |
| **haystack-sgraal** | Python | `pip install haystack-sgraal` | Beta | [`./haystack-sgraal/`](./haystack-sgraal/) |
| **semantic-kernel-sgraal** | Python | `pip install semantic-kernel-sgraal` | Beta | [`./semantic-kernel-sgraal/`](./semantic-kernel-sgraal/) |

## What is Sgraal?

Sgraal is a **memory governance protocol for AI agents.** It evaluates whether your agent's memory state is reliable enough to act on, returning a risk score and a recommended action: proceed, warn, ask the user, or block.

Learn more at [**sgraal.com**](https://sgraal.com):
- [Tutorial](https://sgraal.com/tutorial) — 5-minute walkthrough including the 3 decision bands
- [API reference](https://sgraal.com/docs/api) — full endpoint contract
- [Threat model](https://sgraal.com/docs/threat-model) — what Sgraal catches, doesn't replace, and complements
- [Zero-Knowledge preflight](https://sgraal.com/docs/preflight-zk) — `/v1/preflight/zk` for GDPR / HIPAA / data-residency contexts

## Status legend

- **Production** — substantive integration with tested wrapper surface and field-tested patterns.
- **Beta** — thinner integration (typically <50 LOC); functional but a smaller wrapper surface. Re-classified per the project's [SDK tier reframe](https://github.com/sgraal-ai/sdks).

## License

All SDKs in this repo are licensed under **Apache 2.0**. See [`LICENSE`](./LICENSE).

---

All SDKs are wrappers for the paid Sgraal API. Calibrated scoring requires a Sgraal account. Get one at [sgraal.com](https://sgraal.com).
