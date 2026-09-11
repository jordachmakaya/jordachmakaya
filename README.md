## Hi there 👋

# Jordach Makaya

**Backend engineer — TypeScript · Node.js · NestJS.**

I came to software from insurance claims operations. That is where the bias in everything below comes from: in claims, an unverified assumption has a financial consequence. So I build systems that are deterministic, traceable and auditable.

One rule runs through all of it:

> **VERIFIED ≠ DECLARED.** A task passes only with reproducible proof.

Moving into software full time after building it in parallel since 2021. Open to full-time remote backend roles — contractor (B2B / Deel) or EOR.

📍 Casablanca, Morocco · CET — full EU overlap, 4–5h US East
✉️ jordach@jordach.dev · 🌐 [jordach.dev](https://jordach.dev) · 💼 [LinkedIn](https://www.linkedin.com/in/jordachmakaya/) · 📦 [npmjs.com/~jordach](https://www.npmjs.com/~jordach)

---

## Published packages

All MIT, all public, all built from a problem I actually hit.

| Package | Version | Releases | What it does |
|---|---|---|---|
| [`@hardmachinelabs/index-ai-validator`](https://www.npmjs.com/package/@hardmachinelabs/index-ai-validator) | `0.3.1` | 5 | Validates whether a site correctly exposes an AI-readable layer: `/.well-known/index-ai.json`, `/agent-index.json`, clean Markdown endpoints, declared content size, obvious exposure risks. |
| [`@hardmachinelabs/env-sync`](https://www.npmjs.com/package/@hardmachinelabs/env-sync) | `1.0.1` | 2 | Syncs `.env` variables into GitHub Actions secrets and GitLab CI/CD variables. Monorepo-aware. Built from deployment pain: local, CI and provider secrets drifting apart. |
| [`@hardmachinelabs/zod-config`](https://www.npmjs.com/package/@hardmachinelabs/zod-config) | `0.2.0` | 1 | Runtime configuration validation for TypeScript and NestJS. Zod schemas as the source of truth, fail fast at startup, sensitive values redacted in error output. |

---

## What I am building

Status is stated on every line. Some of this is public and inspectable; some is not yet. I would rather say which than let you assume.

### Shokunin — delivery harness for AI coding agents
**Status: in development · not yet public**

Built on one rule: agent output stays untrusted until deterministic gates verify it.

Designed from a catalogued taxonomy of 40 real coding-agent failure modes — context rot, runaway token spend, compaction loops, unverified commits. It keeps specifications, decisions, jobs, evidence and handoffs *outside* the chat, separates CTO / Coder / Tester / Reviewer roles, loads only the context each task requires, and reports progress through an HTML cockpit.

Implements bounded context routing (in a 500-file reference repository, active context narrows to 8 explicitly routed files), sealed module contracts, mechanical quality gates, SHA-256 artifact sealing and append-only decision ledgers. Traced with Langfuse and OpenTelemetry, evaluated against Harbor / Terminal-Bench.

I use it daily. The human provides intent and judgment; the system carries the process.

### index-ai — an open proposal for AI-readable websites
**Status: open proposal + reference implementation · [public](https://github.com/jordachmakaya/index-ai)**

Websites are built for humans, but agents read differently. Instead of forcing them to scrape noisy HTML, `index-ai` gives them a clean public layer the publisher controls:

- **Agent Manifest** — discovery and site declarations
- **Agent Index** — structured content inventory
- **Agent Graph** — relationships between resources
- **Agent Interface** — queryable access
- Clean Markdown endpoints and measured content size

The goal is not to promise discovery or citations. It is to make agent-facing content publisher-controlled, testable, measurable and verifiable. The validator above is the reference implementation.

### Clausis — claims decision engine (French IRSI convention)
**Status: in development · private**

Backend of a platform turning water-damage claim declarations into step-by-step handling directives. I chose a deterministic rules engine over RAG so every output traces back to a named clause of the *Convention d'Indemnisation et de Recours des Sinistres Immeubles*. NestJS, Mastra AI, SSE streaming, subscription billing with usage metering, SQL analytics.

Comes directly from the job I do by hand.

### Météosure — weather-claim certification for insurers
**Status: in development · private**

Determines whether a severe weather event occurred at a given address on a given date, and returns an adjuster-ready evidence report in under 60 seconds. A Python filtering layer over raw meteorological telemetry, then a NestJS engine applying contractual thresholds. Weekly batch ingestion from Google Drive into Elasticsearch through a three-stage BullMQ/Redis pipeline with Redlock locking and SHA-256 deduplication.

---

## Stack

**Core** — TypeScript · JavaScript · Node.js (v20+) · NestJS · Python · REST · GraphQL · microservices · event-driven architecture
**Data** — PostgreSQL · TypeORM · Prisma · Redis + Redlock · Elasticsearch · Kafka · BullMQ · SQLite
**AI / Agents** — Mastra AI · MCP (tools & servers) · Anthropic, OpenAI and Google AI APIs · Langfuse · RAG · Harbor / Terminal-Bench
**Delivery** — Git · GitHub Actions · GitLab CI/CD · Docker · Dokploy · Nginx · hardened Linux VPS · Cloudflare R2 · OpenTelemetry
**Testing** — Vitest · integration and E2E testing · Zod validation · deterministic CI gates

---

## Writing

- [I Built a CLI to Stop Missing Env Vars from Breaking Deployments](https://dev.to/jordachmakaya/i-built-a-cli-to-stop-missing-env-vars-from-breaking-deployments-59ke) — dev.to

---

## How I work

Map the workflow end to end. Expose the failure points and the missing capabilities. Then build the software required to close the loop.

I keep decision records, failure analysis, test evidence and release criteria, so every claim I make can be inspected.

The goal is not to present experiments as traction. The goal is to show shipped work, clear engineering judgment, and honest status.
