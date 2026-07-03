# 灵枢架构 (LingShu Architecture)

> **"中枢一动，全栈皆通。"**

---

## 📜 灵枢宣言 (The Manifesto)

我们坚持 **Single Source of Truth** 原则。

在灵枢架构中，`reference/` 是所有微服务、前端组件、数据库与 AI Agents 的共同上游。

1.  **中枢权威性**：`reference/docs/` 定义业务真源；代码是文档的投影 (Projection)。
2.  **代码对齐**：代码与文档应保持一致；偏离时及时校正其中一方。
3.  **AI 原生**：本架构在设计上考虑 AI 上下文友好——人类在 `reference/` 中定义"意图"，AI 据此实现。

## 📂 目录结构

- **`rules/`**: **AI 规则真源**。分发到 `CLAUDE.md`、`AGENTS.md` 等产物。
- **`docs/`**: **真源文档**。存储 PRD、API 契约、状态机定义；可按需扩张 `prd/`、`tad/` 等子目录（见 [docs/README.md](./docs/README.md)）。
- **`decisions/`**: **架构决策记录 (ADR)**，可选。仅记录架构决策，不承担计划 / 任务 / 回顾职能；日常任务不写 ADR，走 Git commit 与 PR 描述即可。

---

> [!NOTE]
> 本项目所有对话回复与 Git 提交信息须使用 **简体中文**。
