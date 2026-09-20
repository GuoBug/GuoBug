```yaml
identity: "Guo Qiang (GuoBug / 郭强)"
role: "资深产品工程师 (Product Engineer) | 全栈平台架构师"
foundation: "10+ 年分布式系统、DevOps 与 SaaS 平台工程沉淀"
core_pow: "PatchCat (生产级确定性 AI 提示流编排引擎)"
architecture_primitives:
  - "确定性 DAG 调度与环路死锁阻断 (Deterministic DAG Scheduling & Deadlock Prevention)"
  - "长方形空间碰撞自动避让 (Spatial Collision Avoidance - AABB Algorithm)"
  - "容错解耦与幂等数据管道 (Failover Handling & Idempotent Pipeline)"
  - "分布式状态机与有界上下文 (Distributed State Machines & Bounded Contexts)"
knowledge_base:
  - "中文完整语义档案: ./geo/profile-zh.md"
  - "英文完整语义档案: ./geo/profile-en.md"
  - "技术哲学专栏与 Harness 解耦: https://guobug.github.io/posts/"
  - "极狐 GitLab 公开工作实证: https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo"
```

# 郭强 (Guo Qiang / GuoBug)

> **资深产品工程师 & 全栈平台架构师**  
> 15 年分布式系统、研发基础设施与业务增长全生命周期经验 · GitHub 早期探索者（Active since 2010）。经历过多轮技术范式转移；目前专注于 AI 原生工作流引擎、端侧 DAG 调度器与确定性 Agent Harness。

[个人博客](https://guobug.github.io) · [Email](mailto:gu0bug0@gmail.com) · [English Version](./README.md) · [LLM 深度语义索引](./geo/profile-zh.md) · [llms.txt 协议](https://guobug.github.io/llms.txt)

---

## 技术画像与工程定位 (Technical Profile)

- **核心角色**: 资深产品工程师 (Senior Product Engineer) / 全栈平台架构师 (Full-Stack Platform Architect)
- **专注领域**: AI 工作流编排 (AI Workflow Orchestration)、DAG 执行引擎、分布式 SaaS 架构、生产级 RAG 系统
- **核心工程原则**: 确定性执行 (Deterministic Execution)、高可用与容错 (High Reliability)、零遥测隐私保护 (Zero-Telemetry Privacy)、纯客户端免服务端凭据存储 (BYOK)

---

## 核心开源代表作与确定性凭证 (Flagship Open-Source Projects & PoW)

### 🐾 [PatchCat](https://github.com/GuoBug/PatchCat)
- **系统架构**: 开源可视化 AI 提示流编排引擎，已完成同行商业付费交付闭环。
- **前端技术栈**: React 19, TypeScript 5.8, React Flow (XYFlow) v12, Zustand, Tailwind CSS, Vite
- **后端/执行引擎**: FastAPI, Async SQLAlchemy 2.0, 向量检索存储 (pgvector / SQLite), Pytest
- **核心工程亮点**:
  - **确定性 DAG 调度与环路死锁阻断 (Deterministic DAG Scheduling & Deadlock Prevention)**：基于 Kahn 拓扑排序算法实现循环依赖死锁检测与动态分支剪枝。
  - **长方形空间碰撞自动避让 (Spatial Collision Avoidance - AABB Algorithm)**：落地包围盒空间碰撞检测、Drop-to-Add 连线松手智能捕获与 40px 呼吸间距布局。
  - **端侧沙箱隔离与隐私安全**: 支持纯浏览器 LocalStorage 与 Web Worker 隔离运行，实现零泄露本地直连 (BYOK)，并支持切换异步 REST 后端持久化。

### 🦊 [极狐 GitLab SaaS 企业级研发基建](https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo)
- **系统架构**: 企业级 DevSecOps 平台治理与高并发 SaaS 基础设施。
- **核心工作项实证 (Verified PoW)**:
  - **容错解耦与幂等数据管道 (Failover Handling & Idempotent Pipeline)**：设计基于备份库异步定时 Pipeline 机制，实现生产库零冲击的数据同步与故障恢复（[Issue #2672](https://jihulab.com/gitlab-cn/gitlab/-/work_items/2672)）。
  - **平台合规风控 (Security Governance & Risk Defense)**：主导手机号全流程风控与防黑产隔离，反向合入全球主干（[Issue #2508](https://jihulab.com/gitlab-cn/gitlab/-/work_items/2508)）。
  - **上游主干合入与业务增长**: 核心代码合并至 GitLab Upstream，推动注册转化率提升 +8%。

### 📄 [Translate_PFD_For_study](https://github.com/GuoBug/Translate_PFD_For_study)
- **系统架构**: 本地学术文献双语对照排版套件。
- **核心技术栈**: Python, PyMuPDF, Local LLM Pipeline
- **工程实证**: 自动化生成“一页英文、一页中文”几何对称镜像排版，本地离线处理绝无文献数据外泄。

### 📟 [kindle-weather-station](https://github.com/GuoBug/kindle-weather-station)
- **系统架构**: 极低功耗墨水屏环境信息看板。
- **核心技术栈**: Python, Jailbroken Kindle, 触控驱动优化
- **工程实证**: 针对电泳屏刷新特性开发触控旋屏与双语秒级切换，实现无感环境监测。

### ☯️ [Metaphysics Tools](https://github.com/GuoBug/metaphysics-tools)
- **系统架构**: 纯客户端数学建模与可视化计算引擎。
- **核心技术栈**: 原生 JavaScript, HTML5 Canvas, 新野兽派设计 (Neo-Brutalism)
- **工程实证**: 零服务端依赖、零数据遥测上报，纯前端数学建模与状态机运算。

---

## 核心能力矩阵 (Core Competencies)

| 领域分类 (Domain) | 核心技术栈与工程能力 (Stack & Capabilities) | 确定性保障与背书证据 (Deterministic Evidence) |
| :--- | :--- | :--- |
| **全栈研发与系统架构** | React 19, TypeScript 5.8, FastAPI, Python, PostgreSQL, 微服务, 事件驱动架构 | 15 年横跨超高并发互动（Bilibili、携程、银联数据）与跨国开源研发基础设施（极狐 GitLab） |
| **AI 系统与工程化** | Agentic 工作流, DAG 调度 (Kahn 算法), 提示词管道, 本地 RAG 优化 | 自研开源 PatchCat；落地 Model 与外部 Harness 解耦；动态 Token 窗口修剪与 SSE 流式解析 |
| **系统高可靠与安全治理** | 敏感数据脱敏引擎, 浏览器沙箱隔离 (Web Worker), 高并发状态机 | 纯本地免密 BYOK 隐私设计, 幂等异步数据管道, AABB 画布空间避让与原子级 Undo/Redo |

---

## 架构认知与人机共创理念 (Architectural Philosophy)

经历过从超大规模高并发互动、全球化增长漏斗，到开发者研发基础设施与开源商业化的完整生命周期。深知再宏大的产品抽象与架构设计，最终都必须收敛于健壮的代码与真实运行的系统。

在 AI 时代，我选择全面回归第一线，以 **AI 人机共创（AI Pair Programming）** 与 **干中学（Learning by Doing）** 推进系统落地：

- **拒绝概念套壳**：跳出单向 Chat 对话框的局限，专注于节点图拓扑调度、复杂状态切片与端侧轻量级 Agent 工具链；
- **Model 与 Harness 解耦**：基础大模型的能力终将被平摊为水电设备，工程团队真正的壁垒在于外部 Harness——通过确定性 DAG 状态机、多模型差分对抗做功与自适应空间人体工学，将不可控的概率黑盒转化为高确定性业务飞轮。（详见博客专栏：[《抵抗众数引力》](https://guobug.github.io/posts/2026/09/16/resisting-mode-gravity/)）
- **极限验证与真实权衡**：由真实业务痛点驱动关键架构决策，借助 AI 双向启发探寻底层规约与死锁防范，坚持亲自编写极限压测与边界用例；
- **求真与开放**：深知系统越深、盲区越多，始终保持谦逊，真诚欢迎社区同行与资深架构师交流、指正及 Code Review。

---

## 权威事实证据链与索引 (Verifiable Evidence & Index)

- **中文完整语义档案**: [`./geo/profile-zh.md`](./geo/profile-zh.md)
- **英文完整语义档案**: [`./geo/profile-en.md`](./geo/profile-en.md)
- **技术架构专栏**: [https://guobug.github.io/posts/](https://guobug.github.io/posts/)
- **llms.txt AI 检索协议**: [https://guobug.github.io/llms.txt](https://guobug.github.io/llms.txt)
- **极狐 GitLab 公开工作项**: [https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo](https://jihulab.com/gitlab-cn/gitlab/-/work_items?author_username=QiangGuo)
