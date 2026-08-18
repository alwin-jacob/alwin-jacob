# Alwin Jacob

**AI/ML Systems Engineer · Evaluation · Inference · Reliability**

MS Computer Science, Northeastern University · San Jose, CA

I build **production AI systems at the boundary between model behavior and systems performance**: evaluation infrastructure, LLM inference, reliability tooling, and the software systems that make ML workloads measurable, reproducible, and efficient.

**My Evolving Technical Arc :**
`evaluation → inference → rollout systems → post-training / training infrastructure`

[LinkedIn](https://linkedin.com/in/alwin-jacob) · [Email](mailto:alwinjacob88@gmail.com)

---

## Featured Engineering

### LLM Evaluation & Reliability

**Python · FastAPI · pytest · asyncio · GitHub Actions**

Evaluation and regression infrastructure for models and agents.

* versioned evaluation datasets and reproducible run artifacts
* deterministic, schema, and model-based graders
* independent human-reference and blinded judge experiments
* baseline-vs-candidate regression policies
* timeout, retry, and partial-failure isolation
* concurrent evaluation and provider abstraction
* latency, token, usage, and failure accounting
* CI-tested regression infrastructure

**Engineering question:**
How do we make stochastic model behavior testable with the rigor expected from production software?

→ **[llm-eval-reliability](https://github.com/alwin-jacob/llm-eval-reliability)**

---

### LLM Inference Systems

**vLLM · PyTorch · CUDA · Nsight**

Reproducible benchmarking and performance-analysis infrastructure for LLM serving.

* TTFT, TPOT, throughput, p50 / p95 / p99 latency
* concurrency and request-shape sweeps
* continuous batching behavior
* KV-cache utilization and memory pressure
* prefix caching
* quantization experiments
* speculative decoding
* GPU utilization and bottleneck analysis
* performance regression detection
* controlled cross-runtime experiments

**Engineering question:**
Where does LLM serving performance actually come from — scheduler behavior, memory systems, kernels, or hardware utilization?

**In progress**

---

## Systems Direction

The problems I am most interested in sit across this stack:

```text
Model behavior
      ↓
Evaluation & verification
      ↓
Inference / serving
      ↓
Schedulers, batching & KV cache
      ↓
Distributed execution
      ↓
Compilers & kernels
      ↓
GPU / accelerator hardware
```

Inference also connects naturally back into training:

```text
Inference
    ↓
Rollout generation
    ↓
Rewards / verifiers / evaluation
    ↓
Post-training
    ↓
Distributed training systems
```

Current areas of active depth-building include:

* **Evaluation systems:** regression infrastructure, reliability, judge calibration, agent/tool-use evaluation
* **Inference systems:** batching, KV-cache management, latency/throughput tradeoffs, serving runtimes
* **Performance engineering:** profiling, bottleneck analysis, GPU utilization, reproducible benchmarking
* **Distributed ML systems:** execution, scheduling, communication, fault tolerance
* **Rollout / post-training infrastructure:** inference-backed sampling, evaluation loops, reward/verifier systems
* **Lower-level optimization:** PyTorch internals, Triton/CUDA, kernels, runtime/compiler behavior

---

## Selected Historical Engineering Work

### Fairness-Aware Marketplace Recommendation System

**Project period: 2026 · Public engineering reconstruction / validation ongoing**

**PyTorch · Polars · DuckDB · cvxpy · FastAPI**

End-to-end recommendation and evaluation system exploring relevance versus marketplace exposure.

* implicit-feedback recommendation
* constrained reranking
* recommendation-quality and exposure metrics
* synthetic marketplace simulation
* data-processing pipeline
* API inference
* reproducible evaluation

→ **[Repository](https://github.com/alwin-jacob/fairness-aware-ad-recsys)**

---

### Additional Historical Work

Selected projects from earlier engineering and academic work will be published here with their **original project periods** and clearly identified current reproductions, extensions, or validations where applicable.

The repository publication date is not used as a substitute for the actual period in which historical project work occurred.

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

I am especially interested in systems where **software architecture materially determines model capability, reliability, or efficiency**:

`ML systems` · `inference` · `evaluation` · `AI reliability` · `distributed systems` · `performance engineering` · `rollout infrastructure` · `training systems`

I enjoy working across abstraction boundaries, from model behavior and evaluation methodology down through serving architecture, profiling, runtime behavior, and implementation.
