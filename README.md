<h1 align="center">Hi, I'm Soham Ghodake</h1>

<p align="center">
  <b>Computer Science undergrad @ MIT World Peace University, Pune</b><br/>
  I build distributed systems and AI agent infrastructure.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/soham-ghodake/"><img src="https://img.shields.io/badge/LinkedIn-Soham_Ghodake-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <img src="https://img.shields.io/badge/Location-Pune,_India-555?style=flat" alt="Pune, India"/>
  <img src="https://img.shields.io/badge/Open_to-SDE_/_ML_internships-2ea44f?style=flat" alt="Open to internships / job"/>
</p>

---

###  About me

-  B.Tech Computer Science, MIT World Peace University (2023 – 2027)
-  Most of my work lives where **backend engineering meets AI**: multi-agent orchestration, MCP tooling, consensus, fault injection and observability
-  I like projects that ship with numbers — evals, benchmarks and failure tests, not just demos
-  Co-inventor on a published Indian patent: a smart goggle system that uses ML and EMG sensors to monitor eye twitching in neurological disorders
-  Machine Learning Specialization (Stanford / DeepLearning.AI), ML in Production (DeepLearning.AI), AI Agents (Hugging Face)

---

### 🚀 Featured projects

####  [Hive](https://github.com/sohamghodake/Hive) — self-hosted multi-agent platform
Define an agent as a system prompt plus a scoped set of tools, hand it a task, and watch the run step by step. Agents reach the world only through four **MCP servers** (file, database/RAG, web search, HTTP), and tool permissions are enforced at run time. Every model call, tool call and structured result lands in PostgreSQL.

- **PR reviewer** caught **5/5** planted bugs (SQL injection, cache leak, unawaited async…) with **6/6** correct verdicts
- **0 boundary breaches** across 6 prompt-injection attacks planted in documents and diffs
- **13/13** contract-review quotes grounded verbatim in the source

`Python` `FastAPI` `LangGraph` `MCP` `Next.js` `PostgreSQL + pgvector` `PgBouncer` `Docker Compose`

####  [Ironwork](https://github.com/sohamghodake/Ironwork) — distributed job scheduler in Go
Places and runs jobs across worker nodes with Raft consensus, backpressure, CRDT state, a transactional outbox and mTLS gRPC between services — fully traced and metered.

| Measured on the running cluster | Result |
|---|---|
| Raft leader failover → submissions recover | **1.8 s** median |
| Requests kept during failover | **98.8 %** |
| Worker crash → job reassigned | **8.1 s**, zero job loss |
| CRDT reconvergence after partition heal | **0.22 s** |
| `POST /jobs` latency | **p50 3.9 ms · p99 8.7 ms** |

`Go` `Raft` `gRPC + mTLS` `CRDTs` `PostgreSQL` `Prometheus` `OpenTelemetry` `Jaeger` `Grafana`

####  [rivet-chaos](https://github.com/sohamghodake/Rivet-chaos) — chaos testing for an AI agent runtime
Runs an AI-agent workload on a three-instance Rivet 3.0 cluster, injects **8 fault types** (crashes, pauses, network partitions, storage outages, kill-mid-tool-call) and checks every recorded operation against **8 invariants** from Rivet's documented guarantees. Includes a reproduction of upstream issue #5957 and a dashboard that charts latency with fault windows shaded.

`Rust` `TypeScript` `Docker Compose` `HAProxy` `S3` `Fault injection`

####  [MatchLens](https://github.com/sohamghodake/Match-Lens) — resume → ranked remote jobs
Upload a resume and get ranked remote jobs with a fit score, the reason each matched, the skills you're missing, and an ATS score against any job description. Jobs are ingested daily by a GitHub Actions cron; the app degrades to local models or rules when the LLM is unavailable, and CI runs a Playwright E2E test with the LLM deliberately offline.

`Next.js` `TypeScript` `FastAPI` `PostgreSQL + pgvector` `Groq / OpenAI-compatible LLMs` `Playwright`

####  [FlightCheck](https://github.com/sohamghodake/FlightCheck) — *in progress*
A local-first CLI that inspects an AI app's source code and real HTTP traffic to catch integration mistakes against an LLM provider's API contract, keeping "proven" findings separate from "suspected" ones. Built for the BharatCode Build League.

`Python` `CLI` `HTTP traffic analysis`

---

### Technologies I work with

**Languages:** Python · Go · Rust · TypeScript · SQL · C++ 
**Backend & infra:** FastAPI · gRPC · PostgreSQL · pgvector · Docker · GitHub Actions  
**AI / ML:** LangGraph · Model Context Protocol · RAG · LLM evaluation · Graph Neural Networks  
**Distributed systems:** Raft · CRDTs · transactional outbox · chaos/fault injection  
**Observability:** Prometheus · OpenTelemetry · Jaeger · Grafana  
**Frontend:** Next.js · React

---

<p align="center">
  <i>Currently building FlightCheck and looking for internship / job opportunities — feel free to reach out on my linkedin <a href="https://www.linkedin.com/in/soham-ghodake/">LinkedIn</a> or my email <a href="sohamghodake2005@gmail.com">.</i>
</p>
