# 壹樂 · Jerry

后端为主的全栈工程师，深圳。Java / Python / TypeScript。

五年半时间做过三类东西：面向百万用户的 SaaS 业务系统、重计算与重渲染的行业平台、以及企业级的多模块中后台。近两年重心从前端转到后端与全栈架构，现在在一家上市制造企业做集团级业务平台。

习惯把复杂业务拆成能长期维护的模块，而不是先跑通再说。对性能问题倾向于先量出瓶颈在哪，再决定动缓存、动 SQL 还是动渲染。

## 技术栈

| | |
| --- | --- |
| **后端** | Java 17 / Spring Boot 3、MyBatis-Plus、Sa-Token、OAuth2 & OIDC；Python / Django / DRF |
| **前端** | Vue 2/3（Composition API、Pinia）、TypeScript、React Hooks；GoJS、AG-Grid Enterprise、ECharts |
| **数据与中间件** | PostgreSQL / KingbaseES、MySQL、MongoDB、Redis（多级缓存）、向量数据库 |
| **架构** | 微前端（qiankun）、Monorepo（pnpm / Turborepo）、事务性 Outbox、审批流引擎 |
| **工程化** | Vite / Webpack、Docker、CI/CD（阿里云云效、GitLab CI）、ESLint & Commitlint 规范落地、VitePress 文档体系 |
| **AI 工程** | RAG 全链路（分块、向量化、多路检索）、Agent 意图路由、Tool Calling、会话记忆压缩 |

## 技术实践

**后端与架构**

- 审批流引擎的分层设计：平台内置运行时对外只暴露业务门面与 SPI，业务模块不接触引擎内部。
- 待办的跨系统分发走事务性 Outbox：事件与业务变更同事务落库，由租约式 relay 投递到外部渠道，替掉事务内直接远程调用。
- 实现 OAuth2 / OIDC 身份提供方：授权码、令牌自省与吊销、RP-initiated logout、重定向 URI 校验。
- 百万级数据量下的查询优化：Redis 多级缓存降低数据库 I/O，`CompletableFuture` 并行取多源数据，万人级统计报表通过执行计划调优与中间表预计算解决深度分页与大表关联瓶颈。
- 接入微信支付 V3，配套带补偿机制的异步流程，保证高并发下的最终一致性。
- Python 侧基于 Django + DRF 对接计算引擎，负责多维结果的清洗、重采样与序列化，配合 RBAC 交付业务 API。

**前端与可视化**

- 500–600 节点的行业拓扑图渲染：GoJS 增量更新 + 视口裁剪 + 定制连线算法，渲染性能提升约 70%，交互稳定在 60fps。
- AG-Grid Enterprise 多实例缓存方案，用 GridApi 状态托管解决多表切换的内存激增。
- 微前端 + Monorepo 下的共享组件库建设与包体积优化专项，unplugin 按需引入削减 UI 库体积。
- 拆解业务逻辑高度耦合的上帝组件，用 Composition API 与 JSX 抽离通用逻辑。
- 小程序与 H5 的跨端通信链路（`web-view` + `postMessage`）、分包、虚拟列表与懒加载。
- ECharts-gl 三维可视化大屏，含多分辨率适配。

**AI 工程**

- 跑通「采集 → 清洗 → 分块 → 向量化 → 入库 → 检索」RAG 全链路，实践基于文档结构的分块与稠密 + 稀疏多路检索。
- 会话记忆管理：保留近 N 轮对话并自动摘要压缩，控制 Token 成本同时保持上下文连续。
- 大模型辅助的图形空间布局：传统图论算法在行业接线图上布局失真，改由大模型结合物理约束输出节点路由策略，大幅减少人工调参。

**异构与工程化**

- Meteor 框架从零预研：响应式机制、Turborepo 构建链路与部署流程全生命周期打通；在其上二次开发多租户逻辑隔离与多平台 SSO 免登。
- Electron 桌面端交付，以及 Web 端与条码打印机的集成。
- 电视端遥控器焦点导航与 IE6+ 环境适配（epg-focus、Polyfill、极小内存下的 DOM 精简）。
- 主导 ESLint / Commitlint / GitHooks 规范落地，VitePress 自动化文档体系。

## 教育与背景

统招本科 · 软件工程。Web 前端开发职业技能等级证书（中级）。

现任职于一家上市制造企业，坐标深圳。

## 联系

- Email — ita201125@gmail.com
- GitHub — [@yilecoding](https://github.com/yilecoding)

> 热爱挑战，探究极至。
