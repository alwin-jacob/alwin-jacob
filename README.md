# Alwin Jacob

**AI/ML Systems Engineer · Evaluation · Agent Reliability · Inference**

MS Computer Science, Northeastern University · San Jose, CA

I build inspectable infrastructure for evaluating and operating AI systems. My current public work focuses on failure-aware agent execution and evaluation/regression systems; I am extending this trajectory into LLM inference and serving.

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

## Building Next

### LLM Inference Systems

Reproducible LLM inference and serving infrastructure, beginning with streaming measurement, concurrency, batching, and scheduling behavior. Runtime comparisons, KV-cache analysis, profiling, quantization, and speculative-decoding work will be added only as corresponding implementations and artifacts exist.

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

The goal is a coherent public engineering record in which deeper inspection reveals implementation, tests, reproducible evidence, failures, trade-offs, and explicit limitations.

---

## Selected Historical Engineering Work

### Fairness-Aware Marketplace Recommendation System

**Project period: 2026 · Public engineering reconstruction / validation ongoing**

**PyTorch · Polars · DuckDB · cvxpy · FastAPI**

An end-to-end recommendation and evaluation system exploring relevance versus marketplace exposure through implicit-feedback recommendation, constrained reranking, marketplace simulation, data processing, API inference, and fairness/relevance metrics.

→ **[fairness-aware-ad-recsys](https://github.com/alwin-jacob/fairness-aware-ad-recsys)**

Historical artifacts are identified by their original project periods. Repository publication dates are not presented as substitutes for when earlier work occurred, and current validation or reconstruction is labeled explicitly.

---

## Experience

**Northeastern University**  
Teaching Assistant — Natural Language Processing · Jan 2026 – Apr 2026

**ChargePoint**  
Software QA Engineer Intern — AI/ML Initiative Lead · Jul 2025 – Aug 2025

**Deloitte**  
Consultant · Jul 2022 – Aug 2024

**Tata Institute of Fundamental Research (TIFR)**  
Machine Learning Engineer · Jul 2021 – Jun 2022

---

## Education

**Northeastern University**  
MS, Computer Science · Sep 2024 – May 2026

**University of Mumbai**  
BE, Computer Engineering · Jul 2018 – May 2022

---

## Engineering Interests

`ML systems` · `evaluation` · `agent reliability` · `inference` · `distributed systems` · `performance engineering` · `rollout infrastructure` · `post-training and training systems`
