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

## Beyond the Paper Resume: 14-Year Engineering & Product Odyssey

> Paper resumes are flat—titles can mask mediocrity just as easily as they erase real innovation under extreme constraints. Click any milestone below to read the raw engineering field notes, architectural trade-offs, and commercial lessons:

<details>
  <summary><b>07 / Miaoawu Tech Studio & PatchCat (2024.09 – Present): How 14 Years of Experience & AI Converged into an Open-Source DAG Engine</b></summary>

After leaving JiHu GitLab, instead of immediately jumping into another corporate role, I poured over a decade of engineering, product, and growth experience into my own cross-border private-domain e-commerce business and technical studio.

Initially, operations relied heavily on manual effort. As order volume and customer segments scaled, off-the-shelf platform tools hit a wall. I brought in **AI Workflow Orchestration** and AI Pair Programming: first building automated mini-programs for acquisition and community engagement, then tackling the hardest bottleneck—unifying fragmented orders, logistics, and customer identities across closed, heterogeneous platforms.

Years ago, cross-platform ETL and unified membership mapping would have required a dedicated R&D squad. Pairing with Claude, I evolved the stack step by step: starting with n8n script chains, migrating to Dify, and after hitting state-control limits in generic tools, architecting my own local visual orchestrator powered by a deterministic **DAG Engine** and **State Machine**.

Throughout this milestone co-discovery process, I defined the product ergonomics and operational scenarios (multi-flow drawer isolation, zero-config local LocalStorage privacy execution), while AI helped surface deep algorithmic edge cases (Kahn's topological cycle detection, React Flow 60fps zero-dirty-rerender state slicing, and AABB spatial collision avoidance). After stripping and anonymizing proprietary commerce rules, I open-sourced the core engine as **[PatchCat](https://github.com/GuoBug/PatchCat)**.

With the business pipeline now running autonomously under AI orchestration, my builder's itch to tackle new 0-to-1 challenges is back in full force.

</details>

<details>
  <summary><b>06 / JiHu GitLab (2022.02 – 2024.09): All-Remote Open-Source Culture, SaaS GTM & Strategic Pivot</b></summary>

JiHu GitLab was my first all-remote, international open-source company—and still one of my favorite engineering cultures. Stepping in to lead Ops product lines and China SaaS, I was immersed in GitLab's radical "Dogfooding" ethos, where distributed global teams collaborate asynchronously through transparent handbooks, Issues, and Merge Requests.

To unlock China SaaS growth, I combined platform product engineering with full-funnel GTM mechanics: managing both the official marketing site and developer community, scaling organic acquisition via technical SEO, and overhauling the trial onboarding funnel. Because GitLab's architecture couldn't rely on off-the-shelf third-party trackers, I built an independent telemetry and full-funnel conversion analytics system from scratch, while initiating early enterprise AI DevSecOps explorations.

Later, a top-level corporate strategy shift and executive reorganization led to the sunsetting of local self-developed product lines. Seeing healthy products and painstakingly built funnels zeroed out overnight by macro strategic pivots taught me to evaluate every product line through the lens of corporate cash flow and strategic gravity.

</details>

<details>
  <summary><b>05 / Shanghai Xianze Analytical Instruments (2019.08 – 2022.02): From STM32 Registers & Oscilloscopes to C# .NET Workstation</b></summary>

This chapter was a bold leap into deep-tech hardware: building high-precision pharmaceutical spectroscopy instruments and companion workstation software for research labs. Backed by early commercial intent orders, I dove headfirst from internet software into bare-metal industrial R&D.

In 2019—long before vibe coding—mastering the full hardware-software stack meant starting at STM32 registers and stepper motor drivers: reading datasheets, analyzing timing diagrams, and probing signal waveforms with an oscilloscope whenever a motor stalled. From the bare metal up, I worked across custom real-time scheduling, serial/bus communication protocols, and the C# .NET desktop spectroscopy workstation and lab data platform.

When COVID-19 hit, hardware supply chains froze—even custom mechanical flanges were delayed for months. I took the dev boards and optical modules home to keep debugging firmware and standardizing our Jira R&D workflows. While supply-chain headwinds eventually slowed hardware scaling, that period forged an irreversible confidence: no technical black box is too intimidating to learn from scratch.

</details>

<details>
  <summary><b>04 / Shanghai Qinwen Network · Alo7 (2018.06 – 2019.05): B2B2C Commercialization & User Intent Awakening</b></summary>

After Bilibili, I wanted to step outside pure consumer traffic plays and test myself in B2B2C monetization—joining the innovation arm at Alo7 (Qinwen Network).

We built a full-stack growth and retention suite sold directly to educational institutions: WeChat Mini-Programs driving daily reading check-ins and viral community loops on the front end, backed by a custom-built lightweight CRM, user profiling engine, and licensed video curriculum. Systematic A/B testing lifted registration conversion by over 30%. Around the same period, I also explored offline QR-terminal traffic monetization integrated with major e-commerce APIs (Alibaba/JD), learning firsthand why high-urgency offline micro-moments clash with slow-decision e-commerce rebate funnels.

As regulatory headwinds hit the education sector, the innovation line was scaled back. Stepping outside the traffic greenhouse of mega-platforms taught me a sobering truth: when you no longer have guaranteed organic traffic, matching user psychological intent and macro industry cycles matters far more than feature polish alone.

</details>

<details>
  <summary><b>03 / Bilibili (2016.09 – 2018.03): Crafting a Top-Tier Mobile Web & Facing Strategic Gravity</b></summary>

Joining Bilibili during its hyper-growth phase, I brought my mobile attribution experience from Ctrip to overhaul Bilibili's entire mobile web (H5) platform.

My goal was simple: make it industry-leading. During the architectural rewrite, I proactively embedded channel telemetry and distribution package attribution ahead of business requests. When the marketing team later came asking for campaign tracking, they were stunned to find the entire attribution infrastructure already live. Having end-to-end telemetry also uncovered wild underground anomalies—including third-party pirate apps hotlinking Bilibili's Korean drama video streams to power their own businesses. Once observability is in place, nothing stays hidden.

Yet that excellence created a strategic paradox: strategically, Mobile Web existed as a top-of-funnel acquisition bridge to drive native App installs. The smoother and more complete I made the H5 playback experience, the less incentive users had to download the native App.

It was a defining lesson in product strategy: local craftsmanship always yields to company-level strategic gravity—though proving we could engineer a top-tier high-concurrency mobile web stack remains a proud milestone.

</details>

<details>
  <summary><b>02 / Ctrip (2014.03 – 2016.03): Pioneering Deferred Deep Linking & Cross-BU Attribution</b></summary>

During a 2 a.m. night shift at the bank data center, a casual technical forum chat turned into an interview invite—which turned out to be Ctrip. I joined initially on a hybrid PHP Engineer / Marketing PM contract before transitioning full-time into product management. Having written production code myself meant engineering teams could never bluff me on API contracts or sprint estimates.

Right as James Liang returned to lead Ctrip's mobile-first resurgence, I was handed a foundational challenge: standardizing event telemetry and order channel attribution across 4 fiercely independent Business Units (BUs). After aligning the cross-BU data foundation, I spearheaded two ahead-of-their-time growth engines: a site-wide dynamic H5 engagement system, and seamless H5-to-App invocation preserving full channel context—an early production implementation of Deferred Deep Linking that lifted order conversion across the funnel by 70%~80%.

Building those 0-to-1 growth infrastructures when no industry playbook existed revealed my core DNA: I thrive on 0-to-1 architectural pioneering far more than routine maintenance.

</details>

<details>
  <summary><b>01 / Beijing Lianyintong Tech · SRCB (2012.07 – 2014.01): Linux 0.11 Kernel Roots & Respecting Production Cutovers</b></summary>

My first job after graduation in Shanghai started with an unexpected interview discussion on Linux 0.11 kernel memory management—proving I actually read source code rather than memorizing textbook answers landed me an immediate offer.

Working on the bank's Data Core Platform (IBM DB2 mainframes, C, PL/SQL, and banking middleware) taught me lifelong reverence for the word "Production." On cutover night, less than 10 minutes after traffic switched over, alarms lit up—over 90% of messages jammed in the queue and downstream systems timed out. With the bank's Vice President standing right behind us warning of a full rollback, we traced the bottleneck to an unadjusted queue-width parameter in the production config. Widening the queue and watching the backlog drain in real time was an unforgettable baptism by fire.

Months of 2 a.m. night shifts—waking up to monitor green-on-black terminal `crontab` batch jobs and occasionally spotting a mouse darting across the server room desk—instilled an instinct for operational reliability before I leaped into the rising mobile internet wave.

</details>

---

## Verifiable Evidence & Semantic Index

- **Machine-Readable Semantic Profile (EN)**: [`./geo/profile-en.md`](./geo/profile-en.md)
- **Machine-Readable Semantic Profile (ZH)**: [`./geo/profile-zh.md`](./geo/profile-zh.md)
- **Technical Architecture Essays**: [https://guobug.github.io/posts/](https://guobug.github.io/posts/)
- **llms.txt AI Retrieval Protocol**: [https://guobug.github.io/llms.txt](https://guobug.github.io/llms.txt)
- **Verified Public Issues & MRs**: [https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo](https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo)

