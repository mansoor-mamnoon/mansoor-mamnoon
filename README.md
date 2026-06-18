# Mansoor Mamnoon

**SWE Intern @ Databricks · UC Berkeley EECS Honors, Class of 2027**

Software engineer focused on distributed infrastructure, networking, low-latency C++, and ML security tooling.

[Portfolio](https://mansoor-mamnoon.github.io/) · [Resume](https://mansoor-mamnoon.github.io/resume.html) · [LinkedIn](https://linkedin.com/in/mansoormamnoon) · [Email](mailto:mansoormmamnoon@berkeley.edu)

---

## Background

- **Databricks Traffic Platform** — SWE intern focused on networking, security, and performance infrastructure in Go/Rust.
- **Amazon SDE Intern** — shipped real-time IoT infrastructure processing 10K+ events/min across 100+ sensors with sub-second dashboard latency.
- **UC Berkeley EECS Honors** — CS, GPA 3.973; coursework in OS, compilers, databases, algorithms, ML, and computer architecture.
- **CS 61C Senior Mentor & Content Lead** — wrote worksheets and taught RISC-V, C, caching, pipelining, and memory hierarchy.

---

## Featured Systems

### [LLMFirewall](https://github.com/mansoor-mamnoon/prompt-injection-lab)
MCP security proxy enforcing taint-aware least privilege for tool-using LLM agents.

- Treats prompt injection as a control-flow and policy-enforcement problem across tool calls.
- Seven-layer defense pipeline: capability gating, taint policy, secret-flow guard, argument scanning/sanitization, and output injection checks.
- 4,200+ local eval cases; attack success reduced from 100% to 16% in baseline passthrough setting.

**Stack:** Python · FastAPI · MCP Protocol · NumPy · pytest

---

### [C++20 Limit Order Book + Matching Engine](https://github.com/mansoor-mamnoon/limit-order-book)
Exchange-style matching engine and quantitative replay pipeline.

- Price-time priority matching with FIFO fairness, deterministic replay, snapshot/resume recovery, and strategy tooling (VWAP, TWAP, POV, Iceberg).
- Performance work: slab allocators, branch reduction, cache-hot layouts, CPU pinning.
- 20M+ msgs/sec, p50 ≈ 0.04µs (synthetic benchmark; hardware spec and harness in README).

**Stack:** C++20 · Python · Docker · Streamlit · GitHub Actions

---

### [Edge Deployer](https://github.com/mansoor-mamnoon/edge-deployer)
Zero-config desktop IDE for deploying JS/TS APIs across Cloudflare, AWS, and Vercel.

- Monaco editor, generated infrastructure-as-code, real-time deploy logs, deployment history, and provider-specific environment configuration.
- Built to remove dashboard/CLI context switching from multi-cloud serverless deployment.

**Stack:** TypeScript · Electron · React · Pulumi · Monaco Editor · AWS · Cloudflare · Vercel

---

## Technical Focus

```
Systems / Low-latency       C++20 · C · memory allocators · cache optimization · replay systems
Distributed Infrastructure  Go · Rust · networking · control planes · performance
Backend & Cloud             Python · TypeScript · AWS · Docker · Pulumi · Terraform
ML / LLM Security           MCP · prompt injection defense · taint-aware policies · agent tooling
```

---

Open to 2027 new-grad roles in systems/infrastructure, backend/platform, networking, low-latency, and ML security infrastructure.

`mansoormmamnoon@berkeley.edu` · [mansoor-mamnoon.github.io](https://mansoor-mamnoon.github.io/) · [linkedin.com/in/mansoormamnoon](https://linkedin.com/in/mansoormamnoon)
