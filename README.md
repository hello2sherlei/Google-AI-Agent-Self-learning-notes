# Google-AI-Agent-Self-learning-notes
Google AI Agent课程25天学习资源与笔记

学习目标：

围绕25个主题，4周从零到能在 Google Cloud 上把一个生产级 AI Agent上线。(https://adventofagents.com)


学习计划：


开始前（Day 0）：环境与账户准备 ￼

- 安装并打开：ADK、Agent Engine、Agent Starter Pack。
- 准备 Google Cloud/Vertex AI 与 Gemini 订阅；确认本地 IDE与常用工具链。
- 产出：一个“advent-agents-2025”工作目录，含基础示例项目与云项目可用凭据。

Week 1（Day 1–6）：从零到可运行 ￼￼


|Day|主题                   |关键任务                                                     |产出            |
|---|---------------------|---------------------------------------------------------|--------------|
|1  |Launch Initiative    |明确一个业务场景（如咨询助手/内容整理）；规划25天目标与里程碑。                        |项目说明与路线图      |
|2  |Hello World with YAML|用 YAML 在5分钟内跑起 Gemini 3 的最小Agent，无需写代码。                  |可运行的YAML Agent|
|3  |Gemini 3 + ADK       |在 ADK 中启用搜索实证、计算机使用、实时流。                                 |带搜索/流能力的Agent |
|4  |源码级部署（Agent Engine）  |直接从源码部署，避免序列化问题；熟悉部署命令。                                  |已部署的云端Agent   |
|5  |生产观测（Starter Pack）   |打通 Cloud Trace/Log Analytics/BigQuery；查看一次完整调用链。         |可观测的生产环境      |
|6  |一键就绪的开发环境            |在 Antigravity/Gemini CLI/Cursor/Firebase Studio中跑 ADK 示例。|多环境一致运行记录     |

Week 2（Day 7–12）：上下文、记忆与多模态 ￼￼


|Day|主题                |关键任务                                     |产出            |
|---|------------------|-----------------------------------------|--------------|
|7  |代码执行              |让 LLM 既能写也能执行/调试代码；设计自愈流程。               |具备自主修复能力的Agent|
|8  |上下文管理（ADK Layers） |以“编译视图”组织上下文；拆分与重组层。                     |稳定的上下文层配置     |
|9  |时间旅行/撤销           |为对话实现“编辑消息/重新生成”，不改动数据库结构。               |可回滚的会话状态      |
|10 |大上下文≠好记忆          |接入 Context Caching/Compaction，降低延迟与丢中间问题。|低延迟的上下文策略     |
|11 |Google Managed MCP|通过托管 MCP 连通 Google 服务（Drive/Sheets等）。    |已连接的企业数据      |
|12 |Gemini Live + 双向流 |用 WebSockets 与 Gemini Live 实现多模态双向流。     |实时语音/图像交互Demo |

Week 3（Day 13–18）：状态化工作流、协议与注册 ￼￼


|Day|主题                |关键任务                                       |产出           |
|---|------------------|-------------------------------------------|-------------|
|13 |Interactions API  |从“无状态生成”升级到“有状态自治工作流”。                     |工作流版主代理      |
|14 |Agent2Agent（A2A）  |在 ADK 中实现 A2A；让代理可互联与可发现。                  |可互操作的代理端点    |
|15 |A2UI              |以 JSONL 流式生成 UI，渲染与定义解耦。                   |动态 UI 的前后端对接 |
|16 |LangGraph + A2A   |在 LangGraph 构图中加入 A2A 能力。                  |具备A2A的图式Agent|
|17 |Gemini 3 Flash    |试用可配置“思考层级”；调优速度与质量。                       |快速与稳健的推理配置   |
|18 |API Registry + ADK|用 Cloud API Registry 管理企业工具/API清单并接入 Agent。|中央化工具仓库接入    |

Week 4（Day 19–25）：企业化、扩展与收官 ￼￼


|Day|主题                   |关键任务                     |产出          |
|---|---------------------|-------------------------|------------|
|19 |注册到 Gemini Enterprise|让Agent在组织内可被发现与使用。       |企业级可发现的Agent|
|20 |A2A 扩展 Sidecar       |为特殊数据定义 Sidecar，不破坏兼容。   |自定义数据扩展     |
|21 |Kaggle Capstone      |学习冠军方案要点，评估能否融入你的Agent。  |性能改进点清单     |
|22 |安全与护栏                |采用“模型护甲”，实施真正的治理与数据防护。   |安全策略与测试报告   |
|23 |ADK + Restate 耐久执行   |让Agent可暂停/恢复/抗崩溃，保证上下文不丢。|耐久工作流上线     |
|24 |A2A-ify Anything     |给现有样例一键叠加 A2A 能力（单flag）。 |统一的A2A发布    |
|25 |大结局：架构验收             |汇总架构、观测、安全、耐久与发现性；出一版演示。 |完整演示与复盘文档   |

实操Tips：

- 每日例行：先跑“官方最小示例”，再贴到真实业务场景，最后记录问题与指标。
- 数据与安全优先：Week 2–4同步推进企业数据接入（MCP、Registry）与安全护栏，避免仅靠“提示词约束”。
- 最终交付物：一个“企业可发现 + 可观测 + 可扩展 + 可耐久”的 Agent，附演示视频与操作手册。
