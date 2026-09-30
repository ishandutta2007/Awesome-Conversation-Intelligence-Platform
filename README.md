# Awesome-Conversation-Intelligence-Platform

# 顶级会话智能平台生态系统

**精选 SaaS 产品与开源 GitHub 项目列表**
*聚焦会议录制、语音转写、销售洞察与自动化摘要*
**最后更新：2026 年 9 月**

本仓库追踪 **会话智能** 领域的知名 **SaaS 平台** 与 **开源项目**。这些工具帮助销售、客服和产品团队自动录制会议、转写对话、提取行动项、分析情绪与竞争情报，并将通话数据转化为可操作的收入洞察。

**示例** 包括 Gong、Chorus（ZoomInfo）、Avoma、Fireflies.ai、tl;dv、Jiminny、ExecVision、Salesken、MeetRecord、Fathom、Observe.AI、Otter.ai 和 Grain（该领域的领先者）。

**开源重点**：会话智能的开源生态在 **本地优先转录和摘要** 层面 **快速成熟**。**Meetily** 是当前最受关注的开源方案，拥有 **13.2K GitHub 星标**，完全本地运行 Whisper/Parakeet 模型进行实时转写，Ollama 生成摘要，支持 macOS 和 Windows，MIT 许可 。**Vexa** 提供 Apache-2.0 许可的自托管会议机器人，可加入 Google Meet、Zoom、Teams 并流式传输实时转录 。**Nora** 是面向企业级的多租户会话智能平台，带 PostgreSQL 行级安全、PII 脱敏和 Schema 验证 。**Quill** 提供极简的 macOS 本地录制和转写 。

欢迎贡献！提交 PR 以添加/更新条目。保持描述事实性，并链接到官方网站。

## 目录

- [SaaS/托管平台](#saas托管平台)
- [开源 GitHub 项目](#开源github项目)
- [如何贡献](#如何贡献)
- [免责声明](#免责声明)

## SaaS/托管平台

- **[Gong](https://www.gong.io/)**
  会话智能领域的市场领导者。自动录制和转写销售通话，分析客户情绪、竞争提及和交易风险，提供收入情报和预测。

- **[Chorus（ZoomInfo）](https://www.zoominfo.com/)**
  ZoomInfo 旗下的会话智能平台。提供通话录制、转写、销售辅导和交易洞察，与 ZoomInfo 数据平台深度集成。

- **[Avoma](https://www.avoma.com/)**
  一体化会议助手和会话智能平台。提供会议录制、转写、摘要、行动项提取和收入情报。

- **[Fireflies.ai](https://fireflies.ai/)**
   AI 会议助手。自动加入会议、录制、转写和生成摘要，支持搜索和协作。

- **[tl;dv](https://tldv.io/)**
  会议录制和 AI 摘要工具。提供 Zoom、Google Meet、Teams 录制，时间戳标注和 AI 洞察。

- **[Fathom](https://fathom.video/)**
  免费的 AI 会议助手。自动录制、转写和摘要 Zoom、Meet、Teams 通话，提供即时回顾和行动项。

- **[Otter.ai](https://otter.ai/)**
   AI 会议转写和笔记平台。实时转写、自动摘要、行动项提取，广泛用于会议和采访。

- **[Grain](https://grain.com/)**
  会议录制和洞察平台。提供 AI 摘要、关键时刻剪辑和销售情报。

- **[Observe.AI](https://www.observe.ai/)**
  联系中心会话智能平台。分析客服通话，提供质量保证、合规监控和代理辅导。

- **[Salesloft Conversations](https://salesloft.com/)**
  Salesloft 平台内的会话智能模块。提供通话录制、转写和销售洞察。

## 开源 GitHub 项目

### 本地优先会议助手

- **[Meetily](https://github.com/Zackriya-Solutions/meeting-minutes)**
  **当前最受关注的开源会议笔记工具，13.2K GitHub 星标，MIT 许可。** **完全本地运行**：使用 Whisper 和 Parakeet 模型进行 **4 倍速实时转写**，Ollama 在设备上生成摘要，也可接入 Claude、Groq、OpenRouter 或任何 OpenAI 兼容端点 。**核心特性**：同时捕获麦克风和系统音频，带智能闪避防止音频削波；GPU 加速自动配置（Apple Silicon 的 Metal/CoreML、NVIDIA 的 CUDA、AMD/Intel 的 Vulkan）；支持导入旧录音用更好模型重新转写；原生 macOS 和 Windows 应用，Linux 从源码构建 。**局限性**：免费版 **无说话人标签**（说话人分离在 PRO 版增强），无日历集成，无 PDF/DOCX 导出（PRO $10/月）。

- **[Quill](https://github.com/humanitas-labs/quill)**
  **极简的 macOS 本地录制和转写工具，MIT 许可。** 将麦克风和通话音频录制为独立轨道，在设备上转写，生成带时间戳的 `me`/`them` 转录文本。**完全本地**，不上传任何数据。需要 macOS 15+，推荐 Apple Silicon 以获得转写速度 。

- **[InsightAudio](https://github.com/ggauravky/InsightAudio)**
  **自托管的 AI 会议助手，支持 YouTube 和本地媒体。** 使用 **Whisper 本地转写**（支持 Hindi/Hinglish），**Mistral 生成摘要**、行动项提取，**ChromaDB RAG 聊天**，PDF 导出。**隐私优先**，带 Streamlit 界面 。

### 自托管会议机器人平台

- **[Vexa](https://github.com/Vexa-ai/vexa)**
  **Apache-2.0 许可的自托管会议机器人和智能体平台。** **核心能力**：通过 **API 调用发送机器人加入 Google Meet、Zoom、Teams、Jitsi**，实时流式传输转录（WebSocket 亚秒级交付）；Whisper 支持 **100 种语言** 的多语言转写；**按说话人音频**（无需说话人分离，说话人标签来自平台本身）。**智能体运行时**：临时容器（浏览器/智能体/工作器配置文件），约 5 秒启动；MCP 服务器提供 **17 个工具** 给 Claude、Cursor、Windsurf；知识工作空间自动从会议填充 。**部署**：`make all` 在单台 Linux 主机上通过 Docker Compose 启动完整栈，支持完全气隙环境 。

### 企业级会话智能

- **[Nora](https://github.com/sf0rzin/nora)**
  **面向企业级的多租户会话智能平台。** **架构**：Next.js Web（BFF，API 密钥服务端保留）、Spring Boot API（分层领域/应用/基础设施/API，AWS 风格 IAM，默认拒绝授权）、FastAPI NLP 工作器（调用提供商前先脱敏，Schema 验证输出）。**数据安全**：**PostgreSQL 行级安全已部署强制执行**（API 以 `nora_app` 连接，`NOBYPASSRLS`，即使查询忘记 `tenant_id` 谓词数据库也拒绝跨租户读取）。**Tauri 2 + Rust 桌面客户端** 捕获音频并流式传输到云端转写 。**注意**：前端测试覆盖不均匀，API 启动时若检测到连接仍绕过 RLS 则拒绝启动 。

### 对话情感与上下文分析

- **[CEREBRO (MindShift)](https://github.com/officialarghya29/MindShift)**
  **上下文感知的时间序列对话智能引擎。** **五个理论承诺**：Sentiment ≠ Emotion ≠ Tone（三个正交投影，共享上下文表示上的独立头）；**讽刺检测作为矛盾先验**（正面字面记忆与负面情境期望的对比）；**对话作为时间序列**（情感弧线、马尔可夫链状态转移、鲁棒 z-score 转折点检测、升级轨迹分类）；**融合权重在验证集上调优**（否则披露回退）；**行为信号是温度计而非判决**（响应延迟、CAPS 比率、消息长度坍缩作为支持证据）。**300 msg/s**，CI 验证，可解释。

- **[SideQuest](https://github.com/aechemm/sidequest)**
  **跨对话关系图谱和介绍推荐。** 录制对话（通过 Plaud 或粘贴转录文本），构建 **跨对话的活性关系图谱**，发现单次对话无法揭示的介绍机会。使用 **Crusoe** 进行实体提取，**Neo4j** 存储关系记忆 。

### 其他强开源选项

- **本地优先会议助手**：**Meetily**（13.2K 星标，MIT，Whisper+Parakeet，Ollama），**Quill**（极简 macOS，MIT），**InsightAudio**（Whisper + Mistral + RAG）。
- **自托管会议机器人**：**Vexa**（Apache-2.0，多平台，MCP 17 工具，100 语言）。
- **企业级平台**：**Nora**（多租户，PostgreSQL RLS，Spring Boot + FastAPI）。
- **对话分析**：**CEREBRO**（情感/情绪/语调三维，讽刺检测，时间序列），**SideQuest**（关系图谱，Neo4j）。

**构建自定义系统的框架**：结合 **Meetily** 或 **Quill** 用于本地优先的会议录制和转写，**Vexa** 用于自托管的多平台会议机器人，**Nora** 用于企业级多租户会话智能，**CEREBRO** 用于对话情感和上下文分析，**SideQuest** 用于跨对话关系图谱。添加 **PostgreSQL** 用于持久化，**Neo4j** 用于关系图谱，**Ollama** 或 **Whisper** 用于本地推理。

## 如何贡献

1. Fork 仓库。
2. 在 `README.md` 中添加/编辑条目（遵循现有格式）。
3. 包含：名称、链接、1–2 句描述，以及是 SaaS 还是开源。
4. 提交 PR 并附简短说明。

如果你觉得这个仓库有用，请点星！

## 免责声明

- 这是一个**社区精选**列表——并非详尽无遗，也不构成认可。
- 会话智能平台处理敏感的销售通话和客户对话数据；确保遵守 GDPR、CCPA 和适用的录音同意法规。
- **开源现实**：会话智能的开源生态在 **本地优先会议转写和摘要** 层面 **已经成熟且生产可用**。**Meetily** 以 13.2K 星标和完全本地推理证明了开源方案的可行性 。**Vexa** 提供了 Apache-2.0 许可的自托管会议机器人，支持多平台实时转录 。**Nora** 展示了企业级多租户架构和 PostgreSQL 行级安全的实现 。然而，**商业平台**（Gong、Chorus、Observe.AI）在 **收入情报、交易预测、竞争分析和企业级销售辅导** 方面仍具有显著优势，开源方案需要大量集成和定制开发才能匹配。开源路径最适合 **隐私敏感行业、自托管需求、或作为定制会话智能平台的构建基础**。

---

**为销售团队、收入运营、客户成功和产品经理打造。**
让会话智能更开放、透明、隐私优先。
