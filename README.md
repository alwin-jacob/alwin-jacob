# Alwin Jacob

**AI/ML Systems Engineer · Evaluation · Agent Reliability · Inference**

MS Computer Science, Northeastern University · San Jose, CA

I build infrastructure for evaluating and operating AI systems. My current work focuses on failure-aware agent execution and evaluation/regression systems.

`evaluation → agent reliability → inference / serving → rollout systems → post-training / training infrastructure`

[LinkedIn](https://linkedin.com/in/alwin-jacob) · [Email](mailto:alwinjacob88@gmail.com)

---

## Current Public Engineering

### Agent Reliability Runtime

**Python · LangGraph · asyncio · Pydantic · pytest · GitHub Actions**

A deterministic, failure-aware runtime that makes a small supervisor/worker agent system inspectable from planning through final artifact persistence.

- low-level LangGraph `StateGraph` with supervisor planning/finalization and dynamic two-worker `Send` fan-out
- explicit bounded asynchronous concurrency and typed task-scoped order and return-policy tools
- durable model requests plus per-attempt model/tool evidence, retries, timeouts, typed failures, cancellation, and accepted partial state
- versioned artifacts with strict cross-record validation, schemas, fingerprints, accounting, provenance, and atomic persistence
- 277 deterministic tests and successful GitHub Actions verification on Python 3.11, 3.12, and 3.13

> **Stage 1 boundary:** deterministic local fixtures only. Checkpoint/resume, human approval, MCP, sandboxing, real-provider execution, and external benchmark evidence remain subsequent work.

→ **[agent-reliability-runtime](https://github.com/alwin-jacob/agent-reliability-runtime)**

---

### LLM Evaluation & Reliability

**Python · FastAPI · asyncio · Pydantic · pytest · GitHub Actions**

A local-first evaluation and regression framework for making stochastic model and agent behavior testable with production-software rigor.

- versioned JSONL datasets, strict manifests, and reproducible run artifacts
- provider-independent asynchronous candidates with typed failures, timeouts, bounded retries, and retained attempt history
- deterministic, schema, lexical, and candidate-backed scorers with isolation at example and scorer boundaries
- summaries, slices, baseline/candidate comparisons, and machine-checkable regression policies
- judge/reference agreement analysis with explicit annotation and label provenance
- CLI and local FastAPI interfaces, unit/integration tests, and deterministic CI smoke checks

→ **[llm-eval-reliability](https://github.com/alwin-jacob/llm-eval-reliability)**

---

## Systems Direction

I am interested in systems where software architecture materially determines model reliability, capability, or efficiency:

```text
Model behavior
      ↓
Evaluation and verification
      ↓
Agent execution and reliability
      ↓
Inference and serving
      ↓
Schedulers, batching, and KV cache
      ↓
Rollout and post-training systems
      ↓
Distributed execution, compilers, and kernels
```
---

## Engineering Interests

`ML systems` · `evaluation` · `agent reliability` · `inference` · `distributed systems` · `performance engineering` · `rollout infrastructure` · `post-training and training systems`
