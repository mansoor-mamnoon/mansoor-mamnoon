<div align="center">

# Mansoor Mamnoon

**Systems Infrastructure · Networking · Low-Latency C++ · ML Systems**

[![Portfolio](https://img.shields.io/badge/Portfolio-mansoor--mamnoon.github.io-black?style=flat-square)](https://mansoor-mamnoon.github.io/)
[![Resume](https://img.shields.io/badge/Resume-PDF-555555?style=flat-square)](https://mansoor-mamnoon.github.io/resume.html)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-mansoormamnoon-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/mansoormamnoon)
[![Email](https://img.shields.io/badge/Email-mansoormmamnoon%40berkeley.edu-EA4335?style=flat-square&logo=gmail)](mailto:mansoormmamnoon@berkeley.edu)

</div>

---

**Databricks Traffic Platform SWE Intern** · Previously **Amazon SDE Intern**  
**UC Berkeley CS '27** · EECS Honors Program · GPA 3.973

I build performance-sensitive infrastructure, with a focus on Linux networking, kernel diagnostics, and low-latency systems.

---

## Projects

### [vxlan-tracer](https://github.com/mansoor-mamnoon/vxlan-tracer) — eBPF VXLAN MTU blackhole detector

When an overlay MTU or ICMP path is misconfigured, small requests may work while larger transfers stall, fragment, or repeatedly retransmit. This tool correlates kernel signals to explain why.

- Identifies likely MTU blackholes by correlating fragmentation and ICMP Packet Too Big signals from TC and kprobe programs, without changing application code or network MTU settings
- Reproduces successful path-MTU discovery, ICMP suppression, outer fragmentation, and MTU-mismatch scenarios in network-namespace integration tests
- Validated on amd64 and arm64 across Linux 5.15, 6.8, and 6.10 using CO-RE; auto-detects VXLAN UDP ports via rtnetlink, including standard port 4789 and Flannel port 8472

`Go` `C` `eBPF` `Linux TC` `CO-RE`

---

### [limit-order-book](https://github.com/mansoor-mamnoon/limit-order-book) — C++20 matching engine

Exchange-style order matching engine built for throughput and correctness.

- Implements price-time priority, IOC, FOK, POST_ONLY, self-trade prevention, cancellation, and modification using slab allocation and side-specialized matching paths
- **20.7M order commands/sec** in a single-threaded, in-memory synthetic benchmark; harness, workload configuration, and raw CSV results included in the repository
- Includes deterministic replay and execution-strategy simulation for VWAP, TWAP, POV, and Iceberg orders

`C++20` `Python` `Docker` `GitHub Actions`

---

### [LLMFirewall](https://github.com/mansoor-mamnoon/LLMFirewall) — prompt-injection defense for tool-using LLM agents

MCP security proxy enforcing capability and policy-based controls across tool calls.

- Seven enforcement layers: allowlisting, lookalike detection, argument injection scanning, argument sanitization, secret-flow protection, taint policy, and output-injection checks
- The capability gate categorically prevents retrieved documents from authorizing write-side-effect tools regardless of detection score; adding the gate on top of detection reduces ASR from 73% to 0% on tool-exfiltration attacks
- Evaluated on 4,200+ cases spanning direct injection, indirect RAG injection, tool-output injection, and multi-turn escalation; full pipeline reduces ASR from **100% to 48%** at a **0.6% false-positive rate**; p95 in-process latency 0.15ms, single-thread

`Python` `FastAPI` `MCP` `NumPy` `pytest`

---

### [offline-rl-lab](https://github.com/mansoor-mamnoon/offline-rl-agent) — safety-constrained offline RL benchmark

Standard offline RL optimizes for expected return on benchmark datasets and ignores whether the learned policy is safe to deploy. This project focuses on that gap.

- Six algorithms from scratch (BC, CQL, IQL, TD3+BC, Decision Transformer, AWAC) with consistent interfaces and reproducible benchmark results across 3 seeds
- Offline policy evaluation via FQE, Weighted IS, and Doubly Robust estimators with bootstrap confidence intervals; safety metrics include CVaR-5%, SLO violation rate, OOD action rate, and catastrophic failure rate
- Runtime policy shield with constraint critic and failure explorer for causal analysis of policy failures; built on a 32-dimensional traffic routing simulator with SLO constraints and incident modeling

`Python` `PyTorch` `Streamlit`

---

### [codeglance](https://github.com/mansoor-mamnoon/codeglance) — repo orientation CLI

[![GitHub stars](https://img.shields.io/github/stars/mansoor-mamnoon/codeglance?style=flat-square)](https://github.com/mansoor-mamnoon/codeglance/stargazers)

`npx codeglance` — summarizes what a repository contains, how to run it, and where to start reading. No global install or configuration required.

Detects 50+ frameworks, build systems, and infrastructure tools across Node.js, Python, Go, Rust, C/C++, Java, and Terraform projects from local manifest files. No API keys or LLM calls.

`TypeScript` `Node.js`

---

## Technical Focus

```
Languages       C++ · Go · Rust · Python · TypeScript · C
Systems         Linux · eBPF · TCP/IP · VXLAN · network namespaces · perf
Infrastructure  AWS · GCP · Kubernetes · Docker · Terraform · gRPC
ML / Agents     offline RL · LLM agents · MCP · OPE · safety constraints
Security        prompt-injection defense · capability enforcement · red-teaming
```

---

<div align="center">

**Seeking 2027 new-grad roles in systems infrastructure, networking, low-latency systems, ML systems, and backend platform engineering.**

</div>
