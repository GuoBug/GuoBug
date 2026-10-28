<details>
  <summary><b>🤖 机器可读语义架构元数据 / Machine-Readable Architecture Primitives (LLM Context)</b></summary>

```yaml
identity: "Guo Qiang (GuoBug / 郭强)"
role: "产品工程师 / 产品架构师 (Product Engineer / Product Architect)"
foundation: "14 年分布式系统、DevOps 与 SaaS 平台工程沉淀"
core_pow: "PatchCat（确定性 DAG 工作流引擎）与 FerryCat（确定性 Agent 评测与交接总线）"
architecture_primitives:
  - "确定性 DAG 调度、死锁阻断与预检巡检 (Deterministic DAG Scheduling, Deadlock Prevention & Preflight Lint)"
  - "不可变检查点与反向 BFS 断点续跑 (Resumable DAG Checkpoint & Reverse BFS Resumption)"
  - "契约驱动跨宿主 AI Agent 协作与双智能体评测总线 (MCP + SQLite WAL)"
  - "全文件 SHA-256 指纹防盲审、TOCTOU 软失败缓冲与原子 CAS 租约"
  - "长方形空间碰撞自动避让 (Spatial Collision Avoidance - AABB Algorithm)"
  - "经济模型试探与级联降级状态机 (Cheap-First Model Routing & Cascade Fallback State Machine)"
  - "纯前端零依赖 BM25 + RRF 倒排混合检索 (端侧词法通道)"
  - "后端向量检索 (pgvector) 与可选的远端 Cross-Encoder 重排"
  - "容错解耦与幂等数据管道 (Failover Handling & Idempotent Pipeline)"
  - "分布式状态机与有界上下文 (Distributed State Machines & Bounded Contexts)"
knowledge_base:
  - "中文完整语义档案: ./geo/profile-zh.md"
  - "英文完整语义档案: ./geo/profile-en.md"
  - "技术哲学专栏与 Harness 解耦: https://guobug.github.io/posts/"
  - "极狐 GitLab 公开工作实证: https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo"
```

</details>


# 郭强 (Guo Qiang / GuoBug)

> **产品工程师 / 产品架构师 (Product Engineer / Product Architect)**  
> 14 年角色演进：从写底层代码、理解商业业务，到负责平台产品，再到在 AI 时代重新深入代码、亲手构建自己的确定性系统。目前专注于 AI 原生工作流引擎、端侧 DAG 调度器与确定性 Agent Harness。

[个人博客](https://guobug.github.io) · [Email](mailto:gu0bug0@gmail.com) · [English Version](./README.md) · [LLM 深度语义索引](./geo/profile-zh.md) · [llms.txt 协议](https://guobug.github.io/llms.txt)

---

## 核心开源代表作与确定性凭证 (Flagship Open-Source Projects & PoW)

### 🐾 [PatchCat](https://github.com/GuoBug/PatchCat)
- **系统架构**: 开源可视化 AI 提示流编排引擎，基于纯前端确定性 DAG 状态机实现复杂 Prompt 流转。
- **核心技术栈**: React 18.3, TypeScript 5.7, React Flow (XYFlow) v12, Zustand, FastAPI, Async SQLAlchemy 2.0, pgvector / SQLite, Vite

<details>
  <summary><b>🛠️ 核心工程亮点 / Key Architectural Highlights (展开查看 7 项确定性架构实证)</b></summary>

  - **确定性 DAG 调度与环路死锁阻断 (Deterministic DAG Scheduling & Deadlock Prevention)**：基于 Kahn 拓扑排序算法实现循环依赖死锁检测与动态分支剪枝。
  - **不可变检查点与反向 BFS 断点续跑 (Resumable DAG Checkpoint & Reverse BFS)**：运行失败时向前精准拓扑溯源，仅重跑下游受影响子图，告别整图从头重跑。
  - **长方形空间碰撞自动避让 (Spatial Collision Avoidance - AABB Algorithm)**：落地包围盒空间碰撞检测、Drop-to-Add 连线松手智能捕获与 40px 呼吸间距布局。
  - **经济模型试探与级联降级路由 (Cheap-First Model Routing & Cascade Fallback)**：经济层试探路由，配合三元组诊断反馈与死锁看门狗熔断自愈。30 例 A/B 实测：契约合规率 90.0% → 100.0%，升级率 0% → 10%，Token 开销 +21.8%（配对 McNemar p = 0.25，**未达统计显著**；n = 30，受处理子集仅 3 例）。仅作方向性架构实证，不作为已验证效应。
  - **纯前端零依赖 BM25 + RRF 倒排混合检索 (Zero-Dependency In-Memory Hybrid Retrieval)**：手写 500 行端侧词法检索模块，支持 CJK Bi-gram 分词、参数无关 RRF 融合，并与一个轻量有界启发式相关度分数融合。真实稠密向量检索 (pgvector) 与可选的 Cross-Encoder 重排属于**后端模式**能力，不在零依赖端侧路径内。
  - **画布静态语法巡检与符号仿真 (Flow Preflight Static Lint & Simulation)**：运行前静态 AST 语法树巡检与零 Token 仿真验证，提前拦截断路与幽灵依赖。
  - **端侧沙箱隔离与隐私安全**: 支持纯浏览器 LocalStorage 与 Web Worker 隔离运行，采用设计上不经服务端中转的本地直连 (BYOK) 机制，并支持切换异步 REST 后端持久化。

</details>

### 🛡️ [EdgeCat](https://github.com/GuoBug/EdgeCat) *(正在酝酿)*
- **系统架构**: 本地优先（Local-First）轻量级 AI 推理治理网关，打通端侧本地模型与云端兜底模型调度、流式 PII 脱敏及输出契约治理。（项目尚在酝酿与早期构建中）

### 🚢 [FerryCat](https://github.com/GuoBug/FerryCat)
- **系统架构**: 基于 Model Context Protocol (MCP) 与 Node.js 原生 `node:sqlite`（WAL 并发模式）构建的轻量级、确定性跨宿主 AI Agent 工单交接、代码审查与评测验证底座（Verification Harness）。
- **核心技术栈**: Node.js 22.5+ (`node:sqlite`), TypeScript 5.8, Model Context Protocol SDK, Ajv JSON Schema, Zod
- **确定性工程亮点**:
  - **7 态确定性状态机 (Deterministic 7-State Machine)**：状态流转严格绑定独立 SQL 事务与乐观锁（`changes === 1`），杜绝悬空状态与并发抢单冲突。
  - **全文件 SHA-256 指纹与 TOCTOU 软失败缓冲 (ADR-0004)**：彻底解决桌面不同 IDE Agent（Antigravity、WorkBuddy、Claude Code、Cursor）物理隔离导致的陈旧代码静默盲审难题。
  - **微秒级 CAS 租约受控守护进程 (ADR-0005)**：无写锁探测、短事务 CAS 租约防死锁、子进程树安全回收与声明式白名单脚本调度。
  - **内置静态分析守卫与评测底座**：原生 AST 规则拦截、工作区路径防逃逸与密钥安全检测，支持 SWE-bench 风格的补丁自动化验证。
  - **零配置一键沙箱演练**：单条命令 `npx ferrycat demo` 在 2 秒内完成全流程沙箱闭环自测。

### 🦊 [极狐 GitLab SaaS 企业级研发基建](https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo)
- **系统架构**: 企业级 DevSecOps 平台治理与高并发 SaaS 基础设施。
- **核心工作项实证 (Verified PoW)**:
  - **容错解耦与幂等数据管道 (Failover Handling & Idempotent Pipeline)**：设计基于备份库异步定时 Pipeline 机制，实现生产库零冲击的数据同步与故障恢复（[Issue #2672](https://jihulab.com/gitlab-cn/gitlab/-/work_items/2672)）。
  - **平台合规风控 (Security Governance & Risk Defense)**：主导手机号全流程风控与防黑产隔离，反向合入全球主干（[Issue #2508](https://jihulab.com/gitlab-cn/gitlab/-/work_items/2508)）。
  - **上游主干合入与业务增长**: 核心代码合并至 GitLab Upstream，推动企业新用户首次引导配置完成率提升 +8%。

### 📄 [Translate_PFD_For_study](https://github.com/GuoBug/Translate_PFD_For_study)
- **系统架构**: 本地学术文献双语对照排版套件。
- **核心技术栈**: Python, PyMuPDF, Local LLM Pipeline
- **工程实证**: 自动化生成“一页英文、一页中文”几何对称镜像排版，本地离线处理无需云端上传。

### 📟 [kindle-weather-station](https://github.com/GuoBug/kindle-weather-station)
- **系统架构**: 极低功耗墨水屏环境信息看板。
- **核心技术栈**: Python, Jailbroken Kindle, 触控驱动优化
- **工程实证**: 针对电泳屏刷新特性开发触控旋屏与双语秒级切换，实现无感环境监测。

### ☯️ [Metaphysics Tools](https://github.com/GuoBug/metaphysics-tools)
- **系统架构**: 纯客户端数学建模与可视化计算引擎。
- **核心技术栈**: 原生 JavaScript, HTML5 Canvas, 新野兽派设计 (Neo-Brutalism)
- **工程实证**: 零服务端依赖、无服务端数据中转，纯前端数学建模与状态机运算。

---

## 核心能力矩阵 (Core Competencies)

| 领域分类 (Domain) | 核心技术栈与工程能力 (Stack & Capabilities) | 确定性保障与背书证据 (Deterministic Evidence) |
| :--- | :--- | :--- |
| **全栈研发与系统架构** | React 18.3, TypeScript 5.7, FastAPI, Python, PostgreSQL, 微服务, 事件驱动架构 | 14 年横跨超高并发互动（Bilibili、携程、银联数据）与跨国开源研发基础设施（极狐 GitLab） |
| **AI 系统与工程化** | Agentic 工作流, DAG 调度 (Kahn 算法), 提示词管道, 本地 RAG 优化 | 自研开源 PatchCat（DAG 拓扑调度与局部重放）与 FerryCat（跨宿主 MCP 智能体审查总线、SHA-256 锁定、7 态 WAL 状态机与静态分析守卫） |
| **系统高可靠与安全治理** | 敏感数据脱敏引擎, 浏览器沙箱隔离 (Web Worker), 高并发状态机 | 纯端侧免密 BYOK 隐私设计（无服务端中转）, 幂等异步数据管道, AABB 画布空间避让, 纯前端 BM25+RRF 倒排混合检索与 Cross-Encoder 重排 |

---

<details>
  <summary><b>📐 技术画像与工程定位 (Technical Profile)</b></summary>

- **核心角色**: 产品工程师 / 产品架构师 (Product Engineer / Product Architect)
- **专注领域**: AI 工作流编排 (AI Workflow Orchestration)、DAG 执行引擎、分布式 SaaS 架构、生产级 RAG 系统
- **核心工程原则**: 确定性执行 (Deterministic Execution)、高可用与容错 (High Reliability)、本地优先隐私保护 (Local-First Privacy)、纯客户端免服务端凭据中转 (BYOK)

</details>

<details>
  <summary><b>💡 架构认知与人机共创理念 (Architectural Philosophy)</b></summary>

经历过从超大规模高并发互动、全球化增长漏斗，到开发者研发基础设施与开源商业化的完整生命周期。深知再宏大的产品抽象与架构设计，最终都必须收敛于健壮的代码与真实运行的系统。

在 AI 时代，我选择全面回归第一线，以 **AI 人机共创（AI Pair Programming）** 与 **干中学（Learning by Doing）** 推进系统落地：

- **拒绝概念套壳**：跳出单向 Chat 对话框的局限，专注于节点图拓扑调度、复杂状态切片与端侧轻量级 Agent 工具链；
- **Model 与 Harness 解耦**：基础大模型的能力终将被平摊为水电设备，工程团队真正的壁垒在于外部 Harness——通过确定性 DAG 状态机、多模型差分对抗做功与自适应空间人体工学，将不可控的概率黑盒转化为高确定性业务飞轮。（详见博客专栏：[《抵抗众数引力》](https://guobug.github.io/posts/2026/09/16/resisting-mode-gravity/) · [《纯前端零依赖 BM25 与 RRF 混合检索》](https://guobug.github.io/posts/2026/10/06/ai-prompt-orchestrator-zero-dependency-bm25-and-rrf/)）
- **极限验证与真实权衡**：由真实业务痛点驱动关键架构决策，借助 AI 双向启发探寻底层规约与死锁防范，坚持亲自编写极限压测与边界用例；
- **求真与开放**：深知系统越深、盲区越多，始终保持谦逊，真诚欢迎社区同行与资深架构师交流、指正及 Code Review。

</details>

---

## 纸面履历之外：十余年工程拓荒与职业漫记 (Career Odyssey & Field Notes)

> **14 年角色演进主线**：`2012–2014` 商业银行核心系统与 Linux 底层代码 ➔ `2014–2019` 携程/B站/爱乐奇移动增长与场景心智 ➔ `2019–2024` 工业分析仪器软硬件与极狐 GitLab SaaS 平台治理 ➔ `2024–至今` 全面回归第一线，以一手工程交付 PatchCat 开源确定性 DAG 编排引擎。  
> 纸面履历其实是挺单薄的东西——Title 既能掩盖平庸，也很容易吞掉具体做事的人在极限约束下做的创新与取舍。点击下方各阶段展开对应的工程现场手记，只聊真实的生产现场、架构权衡与商业教训：

<details>
  <summary><b>07 / 喵嗷呜科技工作室 & PatchCat (2024.09 – 至今)：十余年经验与 AI 碰撞，长出开源的 DAG 编排器</b></summary>

从极狐离开后，我将过去十几年的工程、产品与增长经验，投入到了多平台商业化运营与自有技术工作室的研发实践中。

这门业务起初高度依赖人工运营。随着单量和客群规模扩大，现成平台自带的工具彻底不够用了。我开始全面引入 **AI 工作流编排** 与辅助编程（AI Pair Programming）：先快速写出自动化小程序跑通拉新与社群促活；但到了统一管理多渠道分散的订单、物流和客户资产时，撞上了真正的硬骨头——各渠道数据异构且缺乏统一标准。

放在几年前，这种跨渠道异构数据清洗与会员体系打通，非得拉一支专门的研发团队不可。但在与 Claude 等大模型结对编程的过程中，我一步步完成了演化：从最初用 n8n 串联脚本，到过渡至 Dify，再到发现通用工具在复杂状态控制上的局限后，干脆自己动手在本地架构了一套基于 **DAG 状态机** 的可视化编排系统，把多源数据同步、异构用户映射与异常重试跑成了高可靠的 **确定性工作流**。

在这个过程中，我提出业务场景与交互痛点（如多流程抽屉隔离、零配置本地 LocalStorage 隐私运行），AI 协助排查底层工程隐患（如 Kahn 拓扑排序环路死锁规避、React Flow 60fps 零脏重绘状态切片、AABB 空间防碰撞算法）。把涉及具体业务规则的逻辑剥离、脱敏后，我将这套底层核心开源了出来——也就是现在的 **[PatchCat](https://github.com/GuoBug/PatchCat)**（AI Prompt Flow Orchestrator）。

它是过去十几年里，我把底层代码、增长工程、To B/To C 业务体感与 AI 揉在一起后，真真切切从自己手里长出来的作品。随着底层自动化流水线的平稳运转，我将核心精力持续投入在确定性 AI 工作流、端侧 DAG 状态机与下一代 AI-Native 产品架构的深耕与开源演进中。

</details>

<details>
  <summary><b>06 / 极狐 GitLab (2022.02 – 2024.09)：国际化远程开源文化、SaaS GTM 与战略聚焦</b></summary>

极狐 GitLab 是我待过的唯一一家全远程（All-Remote）国际化开源公司，也是我至今非常喜欢的一家公司。做研发的人多少都用过 GitLab 的 CI/CD，进去后我负责 Ops 相关产品线与中国区 SaaS 平台。GitLab 有个我特别喜欢的文化叫“Dogfooding（吃自己的狗粮）”——自己开发工具自己先重度使用，全球跨时区团队全靠极度透明的文档、Issue 和 Merge Request 异步协同。

当时极狐 GitLab 的国内 SaaS 商业化潜力很大，但早期增长还没跑出来。为了把 SaaS 做起来，我把当年市场增长那套 GTM（Go-To-Market）与工程基建本领全拿了出来：对外管官网与技术社区，做渠道与 SEO 拉升自然流量；对内重构注册与 Onboarding 转化漏斗。因为产品架构特殊、无法直接套用现成的第三方统计工具，我干脆自己动手写了一套独立的数据采集与全链路转化分析系统，从流量入口到激活留存全程盯盘。也是在这段时间，我们开始深入探索企业级 AI 研发辅助产品的落地方案。

后来伴随宏观市场环境变化与公司资源向核心底座战略聚焦，部分本土探索业务线进行了战略收敛。这段经历让我深刻体会到：做技术产品不能只看局部功能的完成度，更要学会站在公司现金流、商业ROI与顶层战略矩阵的高度去审视产品生命周期。

</details>

<details>
  <summary><b>05 / 上海仙泽分析仪器 (2019.08 – 2022.02)：跨界硬核仪器研发，从 STM32 寄存器、示波器到上位机架构</b></summary>

这一站跨度很大：一家面向制药与科研院所的分析仪器公司，研发高精度药物光谱分析仪与配套工作站软件。因为前期已有明确的意向订单与极强的行业资源，我决定接下这个挑战，从互联网产品跨入硬核工业软硬件研发。

那还是 2019 年，没有现在的 Vibe Coding。为了把软硬件全链路吃透，我从底层步进电机驱动和 STM32 寄存器啃起：老老实实翻芯片手册、看时序图、调寄存器；电机转不起来，就拿示波器一点点抓波形排查。没有捷径，全靠硬磨。随后一路往上搭：客制化的实时系统调度、上下位机串口/总线通讯协议，再到基于 C# .NET 构建的光谱分析上位机工作站软件与实验室数据管理平台。

期间遇上外部不可抗力冲击，全球硬件供应链一度停滞，连定制的机械法兰都比预期晚到很久。我把开发板和仪器模块搬回家继续调代码、搭 Jira 研发管理体系，硬着头皮把软件架构交付了出来。受限于供应链与长硬件周期，商业化扩张最终放缓；但这段经历给我留下的最大资产是：我再也不怕从零去啃任何硬核的未知技术黑盒了。

</details>

<details>
  <summary><b>04 / 上海钦文网络 · 爱乐奇 (2018.06 – 2019.05)：To B 商业化探索与流量场景心智的顿悟</b></summary>

离开 B 站后，我想跳出纯流量逻辑，去看看真金白银交付的 To B 生意，于是加入了爱乐奇（钦文网络）的创新业务团队。

我们当时做了一套面向教育机构的增长与管理方案：用小程序跑绘本阅读打卡、社群运营与裂变获客，背后配套一套从零搭建的轻量化 CRM 与用户画像系统，再结合权威版权内容与录播课卖给机构。获客、体验、留存转化，链条极短；结合精细化的 A/B 测试，注册转化率拉升了 30% 以上。同期我还深入接触过线下扫码终端与阿里、京东等电商大平台的渠道返利对接，深刻体会到小团队对接巨头平台时的漫长流程，也看清了“急迫场景（如即时租借）”与“慢决策场景（如返利下单）”在用户心智上的天然排斥。

后来随着教培行业外部大盘收紧，新业务线战略收缩。这次经历让我从大厂的流量温室里彻底清醒过来：以前在携程和 B 站，主航道和流量红利是既定的，你只需要把产品细节做好；但脱离了绝对流量的庇护后，场景心智对不对、行业周期站在哪一边，往往比功能本身更决定生死。

</details>

<details>
  <summary><b>03 / 哔哩哔哩 Bilibili (2016.09 – 2018.03)：把移动站体验做到极致，然后直面战略取舍</b></summary>

去 B 站时它正处于高速增长期。我带着携程的移动增长与归因经验过去，接手重构整个 B 站移动 H5 主站。

当时的念头很纯粹：既然做，就做到业内顶级。在架构翻新时，我提前把渠道流量统计、分销渠道包等底层基建全部埋了进去。后来市场部过来提需求，本以为要花很多口舌排期，结果发现他们想要的统计和分发能力全都是现成的。这种提前预判业务演进、把地基先铺好的感觉确实很爽。期间因为数据可观测链路全面打通，我们还通过流量异常监控，精准识别并协助阻断了外部第三方应用恶意盗链视频源流的灰产链路。数据这东西，一旦建成体系，水面下的异常就全都能看见。

但商业上的矛盾也出在这里：H5 在当时公司大盘里的核心定位是获客漏斗——目标是把用户往原生 App 引，而不是让用户留在网页里。所以我把 H5 的播放和交互体验打磨得越丝滑，用户就越缺乏下载 App 的动力。

这是一堂很真实的商业课：在公司的顶层战略面前，局部的极致体验随时需要让路。但我不后悔那段投入，至少证明过自己能把一套高并发前端产品与数据基建打磨到顶级。

</details>

<details>
  <summary><b>02 / 携程 Ctrip (2014.03 – 2016.03)：半夜论坛聊出的 Offer，在蛮荒时代啃下渠道归因与 DeepLink 雏形</b></summary>

在银行核心系统项目交付后的运维阶段，有天半夜值班时在技术论坛跟人交流技术问题，对方说“要不你过来面试看看”，去了才发现是携程。进去时合同签的是 PHP 工程师，一半时间写代码，一半时间做营销产品经理，不久后转为全职产品。因为自己写过底层代码，后来跟研发对齐方案和接口契约时，基本没人能拿技术排期忽悠我。

那会儿正赶上梁建章回归的“二次创业”，全公司重心猛砸移动端。我接到了一个非常底层的硬骨头：在各个业务线（BU）推行基础数据采集和订单渠道归因。当时携程每个大 BU 都有自己的排期利益，我一个人同时面对 4 个核心 BU，带着市场部研发挨个去跟各事业部的产品、研发拉锯对齐。把这套数据地基打下来后，我又牵头落地了两件当时挺超前的事：一是全站多样式 H5 触达引擎；二是 H5 自动唤起 App 并完整保留渠道上下文参数——这其实就是后来行业标配的 DeepLink 延迟归因（Deferred Deep Linking）雏形，直接带动全站相关链路转化率提升 70%~80%。

当年市面上几乎没有现成方案可抄，从 0 到 1 把这几套增长基建跑通并平稳交接后，恰逢处于高速增长期的 B 站伸出橄榄枝，我决定去挑战更大规模的高并发内容分发架构。

</details>

<details>
  <summary><b>01 / 北京联银通科技 (2012.07 – 2014.01)：靠 Linux 内核代码入行，在商业银行核心机房学会敬畏生产环境</b></summary>

毕业后我的第一份工作是到上海后找的。大学时我啃过 Linux 0.11 内核的内存管理模块，面试时聊了对那段源码的理解，面试官觉得不是背八股文的，当场就发了 Offer。

进去后主要驻场参与大型商业银行核心数据聚合平台（DCP）研发，技术栈现在听起来很古典：IBM DB2 主机、C、PL/SQL，外加一堆银行专用中间件。真正让我对“生产环境”四个字产生敬畏，是在一次核心系统割接演练与切流窗口期：所有在文档和代码里看起来很美的东西，只要在生产环境跑不稳，就一文不值。

那次切流窗口刚开启不久监控就触发了告警——高并发消息在队列里出现积压，下游响应逼近超时阈值。现场指挥部气氛极度紧绷，面对随时可能触发熔断回滚的高压窗口，团队火线排查底层配置，迅速定位到是环境切换时一处队列宽度参数未随高并发规格同步放大。当场动态调优队列参数、看着积压数据瞬间平滑泄洪，最终在规定窗口内圆满完成核心割接。

随后几个月在数据中心轮值夜班的经历至今印象很深：凌晨 2 点盯着黑底绿字的终端检查 `crontab` 跑批链路与对账作业是否精准收敛。这段经历把“高可用、强一致与敬畏生产环境”刻进了我的工程基因里。核心项目圆满交付后，看着外面移动互联网正在起势，我决定跳出金融机房看看更大的世界。

</details>

---

## 权威事实证据链与索引 (Verifiable Evidence & Index)

- **中文完整语义档案**: [`./geo/profile-zh.md`](./geo/profile-zh.md)
- **英文完整语义档案**: [`./geo/profile-en.md`](./geo/profile-en.md)
- **技术架构专栏**: [https://guobug.github.io/posts/](https://guobug.github.io/posts/)
- **llms.txt AI 检索协议**: [https://guobug.github.io/llms.txt](https://guobug.github.io/llms.txt)
- **极狐 GitLab 公开工作项**: [https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo](https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo)

