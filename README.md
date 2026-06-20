## Hi there 👋

# Jordach M. Makaya

I build TypeScript systems, developer tools, and AI-assisted workflows.

My current focus is **AI-readable websites**: making public websites easier for AI agents to discover, inspect, and understand through structured metadata, clean Markdown endpoints, and validator tooling.

I also build internal automation systems for deployment, configuration, insurance workflows, and human-in-the-loop AI processes.

---

## What I am building

### index-ai

An open proposal for AI-readable websites.

The idea is simple: websites are built for humans, but AI agents read differently. Instead of forcing agents to scrape noisy HTML, `index-ai` gives them a clean public layer:

* Agent Manifest
* Agent Index
* Clean Markdown endpoints
* Measured content size
* Validator support

Status: open proposal + reference implementation.

### index-ai-validator

A CLI validator for checking whether a website correctly exposes AI-readable metadata.

It validates:

* `/.well-known/index-ai.json`
* `/agent-index.json`
* clean Markdown / text endpoints
* declared content size
* obvious exposure risks

Published on npm under `@hardmachinelabs/index-ai-validator`.

### env-sync

A CLI for syncing `.env` variables into GitHub Actions secrets and GitLab CI/CD variables.

Built from real deployment pain: local variables, CI variables, and provider secrets drifting out of sync.

Published on npm under `@hardmachinelabs/env-sync`.

### zod-config

Type-safe runtime configuration validation for TypeScript and NestJS projects.

It uses Zod schemas as the source of truth, fails fast at startup, and keeps sensitive values redacted in error output.

Published on npm under `@hardmachinelabs/zod-config`.

---

## Published packages

* `@hardmachinelabs/index-ai-validator`
* `@hardmachinelabs/env-sync`
* `@hardmachinelabs/zod-config`

Combined downloads: 700+ across npm packages.

---

## Systems I care about

* TypeScript monorepos
* NestJS / Nuxt applications
* AI agents with structured outputs
* Mastra AI workflows
* CI/CD and deployment automation
* Runtime configuration safety
* Human-in-the-loop insurance workflows
* AI-readable web infrastructure

---

## Current direction

I am preparing the public launch of my portfolio and the `index-ai` proposal.

The portfolio will document the projects behind this work: Meteosure, Clausis, Prospector, Deployment Blueprint, env-sync, zod-config, and index-ai-validator.

The goal is not to present experiments as traction. The goal is to show shipped work, clear engineering judgment, and honest status.
