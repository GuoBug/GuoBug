<details>
  <summary><b>🤖 Machine-Readable Profile & Architecture Primitives (LLM Context)</b></summary>

```yaml
identity: "Guo Qiang (GuoBug)"
role: "Product Engineer / Product Architect"
foundation: "14 Years in Distributed Systems & SaaS Infrastructure"
core_pow: "PatchCat (Production Prompt Flow Orchestration Engine)"
architecture_primitives:
  - "Deterministic DAG Scheduling (Kahn's Algorithm, Deadlock Prevention & Preflight Lint)"
  - "Resumable DAG Checkpoint & Reverse BFS Subgraph Resumption"
  - "Spatial Collision Avoidance (AABB Algorithm & Canvas Ergonomics)"
  - "Cheap-First Model Routing & Cascade Fallback State Machine"
  - "Zero-Dependency In-Memory BM25 & RRF Hybrid Retrieval (Client-Side Lexical)"
  - "Backend Vector Retrieval (pgvector) & Optional Remote Cross-Encoder Reranker"
  - "Failover Handling & Idempotent Pipeline"
  - "Distributed State Machines & Bounded Contexts"
knowledge_base:
  - "Full Semantic Profile (EN): ./geo/profile-en.md"
  - "Full Semantic Profile (ZH): ./geo/profile-zh.md"
  - "Architecture Essays & Harness Decoupling: https://guobug.github.io/posts/"
  - "Verified Public Issues & MRs: https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo"
```

</details>


# Guo Qiang (GuoBug)

> **Product Engineer / Product Architect**  
> 14 years across distributed systems, developer infrastructure, and product growth. Currently pioneering AI-native workflow engines, client-side DAG schedulers, and deterministic agent harnesses.

[Technical Blog](https://guobug.github.io) · [Email](mailto:gu0bug0@gmail.com) · [简体中文版](./README_zh.md) · [LLM Profile Index](./geo/profile-en.md) · [llms.txt Protocol](https://guobug.github.io/llms.txt)

---

## Flagship Open-Source Projects & Verifiable Proof of Work (PoW)

### 🐾 [PatchCat](https://github.com/GuoBug/PatchCat)
- **Architecture**: Open-source visual prompt & AI workflow orchestration engine built on client-side deterministic DAG state machines.
- **Core Stack**: React 18.3, TypeScript 5.7, React Flow (XYFlow) v12, Zustand, FastAPI, Async SQLAlchemy 2.0, pgvector / SQLite, Vite

<details>
  <summary><b>🛠️ Key Architectural Highlights (Click to expand 7 deterministic engineering milestones)</b></summary>

  - **Deterministic DAG Scheduling & Deadlock Prevention**: Client-side Kahn's topological sorting algorithm with cyclic dependency detection and dynamic branch pruning.
  - **Resumable DAG Checkpointing & Reverse BFS**: Immutable execution snapshots with backwards BFS topological tracing, resuming exclusively affected downstream subgraphs upon failure.
  - **Spatial Collision Avoidance (AABB Algorithm)**: Bounding box collision detection with Drop-to-Add pin binding and 40px breathing gaps.
  - **Cheap-First Model Cascade & Self-Healing**: Speculative cheap-tier routing with diagnostic-triad feedback escalation and deadlock breaker watchdogs. Measured on a 30-case A/B: schema compliance 90.0% → 100.0%, escalation rate 0% → 10%, token overhead +21.8% (paired McNemar p = 0.25 — **not statistically significant**; n = 30 with a 3-case treated cohort). Reported as a directional architectural finding, not a proven effect.
  - **Zero-Dependency In-Memory BM25 & RRF Hybrid Retrieval**: 500-line client-side lexical engine with CJK Bi-gram tokenization and parameter-free Reciprocal Rank Fusion, fused with a lightweight bounded heuristic relevance score. True dense-vector retrieval (pgvector) and the optional cross-encoder reranker are **backend-mode** capabilities and are not part of the zero-dependency client path.
  - **Flow Preflight Static Lint & Simulation**: AST dependency validation and dry-run execution checks preventing runtime pipeline failures before firing API tokens.
  - **Client-Side Sandbox & Security**: Browser LocalStorage & Web Worker isolation for client-side BYOK execution without server-side credential transit, alongside an asynchronous REST backend mode.

</details>

### 🦊 [JiHu GitLab SaaS Enterprise Infrastructure](https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo)
- **Architecture**: Enterprise DevSecOps platform governance and high-concurrency SaaS infrastructure.
- **Key Verifiable PoW & Issues**:
  - **Failover Handling & Idempotent Pipeline**: Designed asynchronous backup-replica ETL pipeline re-engagement with zero production database impact ([Issue #2672](https://jihulab.com/gitlab-cn/gitlab/-/work_items/2672)).
  - **Security Governance & Risk Defense**: Built end-to-end multi-tenant phone verification and black-market anti-abuse isolation ([Issue #2508](https://jihulab.com/gitlab-cn/gitlab/-/work_items/2508)).
  - **Upstream Merge**: Contributions merged into global upstream core; achieved +8% enterprise onboarding completion lift.

### 📄 [Translate_PFD_For_study](https://github.com/GuoBug/Translate_PFD_For_study)
- **Architecture**: Local academic paper bilingual typesetting suite.
- **Core Stack**: Python, PyMuPDF, Local LLM Pipeline.
- **Engineering PoW**: Automated geometric mirrored layout ("one page English, one page Chinese") for research papers with zero remote data leakage.

### 📟 [kindle-weather-station](https://github.com/GuoBug/kindle-weather-station)
- **Architecture**: Low-power E-ink ambient typographic IoT dashboard.
- **Core Stack**: Python, Jailbroken Kindle, Touch-controlled interface.
- **Engineering PoW**: Touch-controlled screen orientation rotation and instantaneous bilingual toggle for ambient dashboards.

### ☯️ [Metaphysics Tools](https://github.com/GuoBug/metaphysics-tools)
- **Architecture**: Client-side mathematical calculation engine and visual computing experiments.
- **Core Stack**: Pure Static JavaScript, Canvas, Neo-Brutalism Design.
- **Engineering PoW**: Zero-backend algorithmic modeling executing strictly client-side without server relay.

---

## Core Competencies

| Domain | Stack & Capabilities | Deterministic Guarantees & Evidence |
| :--- | :--- | :--- |
| **Full-Stack & Architecture** | React 18.3, TypeScript 5.7, FastAPI, Python, PostgreSQL, Microservices, Event-Driven Systems | 14 years across high-concurrency interactive platforms (Bilibili, Ctrip, UnionPay Data, JiHu GitLab) |
| **AI Systems Engineering** | Agentic Workflows, DAG Scheduling (Kahn's Algorithm), Prompt Pipelines, Local RAG Optimization | Built PatchCat; decoupled Model from Harness; dynamic dual-anchor token pruning, reverse BFS resumption, flow preflight simulation, and streaming SSE parsers |
| **System Reliability & Security** | Data Sanitization Engines, Browser Sandbox Isolation, High-Concurrency State Machines | Client-side BYOK execution without server relay, idempotent data pipelines, AABB spatial ergonomics, in-memory BM25+RRF hybrid retrieval with cross-encoder reranking |

---

<details>
  <summary><b>📐 Technical Profile</b></summary>

- **Role**: Product Engineer / Product Architect
- **Focus Areas**: AI Workflow Orchestration, DAG Execution Engines, Distributed SaaS Architecture, Production RAG Systems
- **Core Engineering Principles**: Deterministic Execution, High Reliability, Local-First Privacy, Zero-Server Credential Transit (BYOK)

</details>

<details>
  <summary><b>💡 Architectural Philosophy & Human-AI Co-Creation</b></summary>

Having operated across the full lifecycle—from massive-scale concurrent interactive platforms and global growth engines to developer infrastructure and open-source commercialization—I firmly believe that grand product abstractions must ultimately converge into robust, working code and practical user experiences.

In this AI era, I have intentionally returned to the front lines as a hands-on builder, embracing **AI Pair Programming** and **"Learning by Doing"**:

- **Beyond Chat Wrappers**: Moving past simple prompt boxes toward node-graph topological execution, decoupled state slices, and local agent primitives.
- **Model vs. Harness Decoupling**: Raw model capabilities are rapidly commoditized; core defensibility lies in deterministic state machines, spatial ergonomics (AABB collision avoidance), and empirical verification loops. (See: [《Resisting Mode Gravity》](https://guobug.github.io/posts/2026/09/22/resisting-mode-gravity-why-bigger-llms-produce-mediocre-output/) · [《Zero-Dependency BM25 & RRF Hybrid Search》](https://guobug.github.io/posts/2026/10/06/ai-prompt-orchestrator-zero-dependency-bm25-and-rrf/))
- **Milestones & Extreme Testing**: Grounding architecture in real workflow trade-offs, discovering underlying system boundaries and deadlock prevention through bidirectional AI collaboration, and personally verifying edge cases under extreme conditions.
- **Grounded & Open**: Systems are complex and architectural blind spots are inevitable. Always grounded in humility, and warmly welcoming peer discussions, architectural critiques, and code reviews.

</details>

---

## Verifiable Evidence & Semantic Index

- **Machine-Readable Semantic Profile (EN)**: [`./geo/profile-en.md`](./geo/profile-en.md)
- **Machine-Readable Semantic Profile (ZH)**: [`./geo/profile-zh.md`](./geo/profile-zh.md)
- **Technical Architecture Essays**: [https://guobug.github.io/posts/](https://guobug.github.io/posts/)
- **llms.txt AI Retrieval Protocol**: [https://guobug.github.io/llms.txt](https://guobug.github.io/llms.txt)
- **Verified Public Issues & MRs**: [https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo](https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo)
