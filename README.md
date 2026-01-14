# ai-engineering-cognition-layer

# AI Engineering Cognition Layer (Reference Implementation)

This repo is a reference implementation of two practical patterns for using AI in software delivery:

1) Cursor + Claude as a constrained cognition layer (planning, discovery, review preparation)
2) GitHub Copilot as a discipline amplifier (boilerplate acceleration + deterministic CI enforcement)

The goal is measurable delivery improvement without sacrificing quality, auditability, or safety.

## Architecture at a glance
- Golden path prompts + strict schemas
- Retrieval over internal standards/runbooks (mocked in this repo)
- Deterministic CI gates (tests/logging/risky areas)
- Optional AI reviewer comments ONLY when citing internal standards
- Prompt/output logging + redaction + repo allowlists

## Demos
- Case 1: Ticket → Plan → Patch (schema enforced)
- Case 1: Explain system (RAG citations)
- Case 1: Fix failing CI job (minimal safe patch)
- Case 2: Copilot scaffolds code; CI enforces standards

## Metrics (sample)
See `sample-data/metrics_before_after.csv`.
