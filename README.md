<div align="center">

<img src="./assets/hero.svg" width="100%" alt="壹樂 · Jerry —— 后端为主的全栈工程师 · 深圳"/>

<br/>

<a href="mailto:ita201125@gmail.com"><img src="https://img.shields.io/badge/Email-0c1222?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>

</div>

<br/>

### 👋 你好，我是壹樂

后端为主的全栈工程师，坐标深圳。

- 🧭 **五年半**：前端起步，近两年重心转到后端与全栈架构
- 🏭 **现在**：在一家上市制造企业做集团级业务平台
- 🎯 **擅长**：后端架构设计 · 复杂业务拆解 · 全链路性能调优 · AI 应用工程 · 大规模数据可视化
- 🎓 **背景**：统招本科 · 软件工程
- 💌 **联系**：[ita201125@gmail.com](mailto:ita201125@gmail.com)

<table>
  <tr>
    <td width="33%" valign="top">
      <b>🏗️ 先拆清楚，再动手</b><br/>
      <sub>审批流、跨系统分发、身份认证，都先划清边界和分层，再谈实现。</sub>
    </td>
    <td width="33%" valign="top">
      <b>🚀 性能用数字说话</b><br/>
      <sub>百万级数据查询调优；600 节点拓扑渲染提速 70%，稳定 60fps。</sub>
    </td>
    <td width="33%" valign="top">
      <b>🧠 AI 落到工程里</b><br/>
      <sub>RAG、Agent、MCP 不止做 demo，还要管住检索质量和 Token 成本。</sub>
    </td>
  </tr>
</table>

<br/>

## 🛠️ 技术栈

<div align="center">

<img src="https://skillicons.dev/icons?i=java,spring,py,django,fastapi,ts,vue,react,vite,tailwind&theme=dark" alt="语言与框架"/>
<br/>
<img src="https://skillicons.dev/icons?i=electron,postgres,mysql,mongodb,redis,docker,gitlab,githubactions,linux&theme=dark" alt="数据与工程化"/>

</div>

<br/>

| | |
| :-- | :-- |
| **后端 · Java** | `Java 17` `Spring Boot 3` `Spring Security` `MyBatis-Plus` `Sa-Token` `OAuth2 / OIDC` |
| **后端 · Python** | `FastAPI` `Pydantic 2` `SQLAlchemy 2（async）` `Alembic` `Celery` `Django / DRF` |
| **前端** | `Vue 2/3` `Pinia` `React 19` `TypeScript` `TanStack Router / Query / Table` `Tailwind CSS` `shadcn/ui` `zustand` `i18next` |
| **可视化** | `ECharts / ECharts-gl` `GoJS` `AG-Grid Enterprise` |
| **多端** | `Electron` `Expo / React Native` `小程序` `H5` |
| **数据与存储** | `PostgreSQL / KingbaseES` `MySQL` `SQL Server` `MongoDB` `Redis` `向量数据库` `S3 对象存储` |
| **架构** | `微前端 qiankun` `Monorepo（pnpm + turbo）` `事务性 Outbox` `审批流引擎` `RBAC + 行级数据权限` `Socket.IO 实时推送` |
| **工程化** | `Vite` `Docker` `GitLab CI` `GitHub Actions` `阿里云云效` `uv / ruff` `VitePress` |
| **测试** | `pytest` `Playwright 端到端` |
| **AI 工程** | `RAG 全链路` `分块策略` `Embedding` `稠密 + 稀疏多路检索` `Agent 意图路由` `Tool Calling` `MCP` `pydantic-ai` `会话记忆压缩` `Prompt 工程` |

<br/>

## ⚙️ 做过的事

- ⚙️ 审批流引擎分层设计，运行时对外只暴露业务门面与 SPI
- 📤 待办跨系统分发走事务性 Outbox + 租约式 relay，替掉事务内远程调用
- 🔐 实现 OAuth2 / OIDC 身份提供方，含令牌自省、吊销与登出
- 🚀 百万级数据查询优化，Redis 多级缓存 + 执行计划调优 + 中间表预计算
- 🕸️ 600 节点行业拓扑图渲染提速 **70%**，稳定 60fps
- 🧠 RAG 全链路自建：分块 → 向量化 → 入库 → 稠密 + 稀疏多路检索
- 🤖 大模型辅助图形空间布局，替代失真的传统图论算法
- 🔌 MCP 下的工具动态调用与长程会话记忆压缩，控 Token 成本

<details>
<summary><b>展开更多技术实践</b></summary>

<br>

**后端**

- `CompletableFuture` 并行取多源数据；万人级统计报表解决深度分页与大表关联瓶颈
- 微信支付 V3 接入，配套带补偿机制的异步流程保证最终一致
- Django + DRF 对接计算引擎，负责多维结果的清洗、重采样与序列化，配合 RBAC 交付 API

**前端与可视化**

- GoJS 增量更新 + 视口裁剪 + 定制连线算法
- AG-Grid Enterprise 多实例缓存，GridApi 状态托管解决多表切换内存激增
- 微前端 + Monorepo 共享组件库建设，unplugin 按需引入削减包体积
- 拆解耦合严重的上帝组件，用 Composition API 与 JSX 抽离通用逻辑
- 小程序与 H5 跨端通信（`web-view` + `postMessage`）、分包、虚拟列表
- ECharts-gl 三维可视化大屏，含多分辨率适配

**AI 工程**

- 跑通「采集 → 清洗 → 分块 → 向量化 → 入库 → 检索」全链路
- 稠密 + 稀疏多路检索，基于文档结构的分块策略
- 会话记忆压缩：保留近 N 轮并自动摘要，控 Token 成本同时保上下文连续

**异构与工程化**

- Meteor 框架从零预研，构建链路与部署全生命周期打通；二次开发多租户隔离与 SSO 免登
- Electron 桌面端交付、Web 端条码打印机集成
- 电视端遥控器焦点导航与 IE6+ 适配（epg-focus、Polyfill、极小内存 DOM 精简）
- 主导 ESLint / Commitlint / GitHooks 规范落地与文档体系建设

</details>

<br/>

<img src="./assets/footer.svg" width="100%" alt="热爱挑战，探究极致。"/>
