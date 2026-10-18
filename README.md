# Jeff Hoffman

Senior software engineer in Charlotte, NC. I specialize in enterprise API integrations and agent-orchestrated software development.

## Background

I spent 5½ years at Transcend building across the full stack of a privacy platform — data-rights infrastructure, third-party integrations, and admin and customer-facing product surfaces — and the last ten months on the Integrations team that owns its catalog of 1,500+ third-party connectors: the OAuth flows, rate limits, polling, bulk exports, retries, and vendor-specific failure modes that make integrations hard to run reliably at scale. Over those years I merged 360 production PRs.

In 2026 I led the team's shift to agent-orchestrated development. 89% of my merged production PRs were agent-authored (up from 8% in 2025) while my merge velocity roughly doubled. The guardrails that made that safe in a regulated codebase: recorded-mock tests with sanitized HTTPS capture and deterministic replay, a code-simplification subagent that keeps machine-written diffs reviewable, and human review on every merge.

Earlier: twelve years as CTO of two software companies, and three years leading UNC Charlotte's full-stack bootcamp (300+ graduates). I have 20+ years shipping production software and returned to hands-on engineering by choice.

## What I'm building

AI systems that can show where their answers came from and be tested when models or retrieval strategies change. The current project is an NC Medicaid policy retrieval agent over a Neo4j knowledge graph: every answer cites a primary source, unsupported claims are rewritten in place, and an evaluation harness (golden dataset, precision/recall/MRR, CI-enforced model A/B) gates every release.

Recent client work (private): FiduciCalc — a 1980s-era C planned-giving actuarial library ported to pure Rust, verified against the legacy binary through an FFI parity-test layer, and shipped as a REST API and MCP server behind a spec-compliant OAuth 2.1 authorization server.

## Selected public work

- **[agent-procs](https://github.com/jkhoffman/agent-procs)** — Rust process supervisor for agent-driven development: daemon persistence across CLI invocations, dependency-ordered startup, readiness checks, durable logs, restart policies.
- **Hermes Agent (Nous Research)** — contributor. Merged [#94995](https://github.com/NousResearch/hermes-agent/pull/94995): remote MCP servers returning an empty `cacheScope` were failing SDK schema validation and aborting tool discovery; added a narrowly scoped pre-validation compatibility shim for the list methods, with tests. I run Hermes Agent self-hosted, which is how I hit it.
- **[DoTheHardThing](https://github.com/Queen-City-Cortex/DoTheHardThing)** — a mobile-first daily focus PWA: name what's uncomfortable, pick one thing, protect one block. Live at [dothehardthing.app](https://dothehardthing.app).

## Contact

Open to senior and lead engineering roles in integration platforms, privacy and data-governance tech, and AI-enabled product engineering, and to contract work through [Queen City Cortex LLC](https://queencitycortex.com). Remote or Charlotte, NC.

[LinkedIn](https://www.linkedin.com/in/jkhoffman) · jkhoffman@gmail.com
