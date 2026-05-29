# Alomana Lab

We design reliable autonomous systems.

AI agents that run continuously, in production, against real data, and don't break in ways you can't reason about.

---

## What we're working on

Autonomous agents fail in predictable ways: context bloat, structured output drift, brittle tool orchestration, silent degradation under load. We study these failure modes systematically and build the infrastructure to prevent them.

Our work spans:

- **Evaluation environments** — reproducible test harnesses for autonomous systems that capture production failure modes, not just benchmark accuracy
- **Structured output reliability** — why models with high reasoning accuracy still produce near-zero usable output, and how to fix it without fine-tuning
- **Context management for long-horizon agents** — token-aware compaction, pre-trimmed tool outputs, sidecar extraction patterns
- **Agentic orchestration primitives** — lightweight patterns for multi-step, multi-model workflows that are inspectable and recoverable

---

## Research

**[When Correct Isn't Usable: Improving Structured Output Reliability in Small Language Models](https://arxiv.org/abs/2605.02363)**  
arXiv 2605.02363 · 2026

Core finding: small language models can achieve near-perfect reasoning accuracy while producing structurally invalid output on the vast majority of responses. Accuracy metrics don't capture what actually breaks in production. We introduce AloLab — an evaluation framework that measures output usability, not just correctness — and demonstrate strong output reliability without fine-tuning.

---

## Design philosophy

**Reliable before capable.**  
A system that fails unpredictably is worse than a system with narrower scope. We start from failure modes and work backwards.

**Environments matter as much as models.**  
Most evaluation is contaminated by the gap between benchmark conditions and deployment conditions. We build evaluation environments that reproduce what actually happens when agents run in the wild — context pressure, malformed inputs, cascading tool errors.

**Models deserve rigorous engineering.**  
The frontier isn't the constraint for most real workloads. We care about what you can actually run, control, and audit.

**Transparency about failure.**  
Our most useful findings have come from systems that didn't work. We publish those too.

---

## Background

Alomana Lab is the research and open source arm of [Alomana](https://alomana.com), an enterprise AI company building autonomous agent systems for enterprises. Our tooling is extracted from production deployments, hardened, and released.

---

## Get involved

If you're working on agent reliability, evaluation environments, or structured generation in constrained models — we're likely solving adjacent problems.

Open an issue. Cite the paper. Reach out at [lounge@alomana.com](mailto:lounge@alomana.com).
