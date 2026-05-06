# ⚙️ Harness Engineering Skills

> **一套面向 Cursor 的 Agent Skill 合集**：Harness 方法论、分版本规划、可执行指南与两类「图谱」分析——让代理在**有边界、有证据、少扫仓**的前提下干活。

[![Cursor](https://img.shields.io/badge/Cursor-Agent%20Skills-000000?logo=cursor&logoColor=white)](https://cursor.com)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/RonnyJung2021/harness-engineering-skill/pulls)

---

## 📋 这是什么

本仓库在 `skills/` 下收录多份 **Cursor Agent Skill**（每份以目录为单位，入口一般为 `SKILL.md`）。它们共享同一套工程观：**模型提供智能，Harness（环境系统）提供可控制、可验证的确定性**。

```
╔═══════════════════════════════════════════════════════╗
║         Agent = Loop(Model + Harness)                 ║
║     模型可替换；约束、反馈与验证应落在环境里           ║
╚═══════════════════════════════════════════════════════╝
```

| | |
|:--|:--|
| ✅ **适合** | 想系统搭建 Agent、先画图再写码、把大项目拆成可交付版本、把模糊需求变成可粘贴执行的步骤 |
| ❌ **不适合** | 指望单一 prompt 解决一切、跳过验收与边界讨论 |

---

## 📦 `skills/` 里有什么

| 目录 | `SKILL.md` 中的 `name` | 一句话 | 文档入口 |
|------|------------------------|--------|----------|
| [`harness-engineering`](skills/harness-engineering/) | `harness-engineering` | Harness 八大要素与五层架构，指导可生产 Agent 的设计与加固 | [README](skills/harness-engineering/README.md) · [SKILL.md](skills/harness-engineering/SKILL.md) · [中文版说明](skills/harness-engineering/README.zh.md) |
| [`harness-guide-generator-skill`](skills/harness-guide-generator-skill/) | `vibe-coding-harness-guide-generator` | 把自然语言任务变成可复制到 Agent 的分步指南与验收标准 | [README](skills/harness-guide-generator-skill/README.md) · [SKILL.md](skills/harness-guide-generator-skill/SKILL.md) |
| [`large-project-versioned-roadmap`](skills/large-project-versioned-roadmap/) | `large-project-versioned-roadmap` | 大型工程按纵向主路径或横向模块拆成多版本路线图与技术选型建议 | [SKILL.md](skills/large-project-versioned-roadmap/SKILL.md) |
| [`project-atlas-analyzer-skill`](skills/project-atlas-analyzer-skill/) | `repository-atlas` | 不绑定具体需求，把当前仓库浓缩成可反复引用的 Markdown 图谱 | [README](skills/project-atlas-analyzer-skill/README.md) · [SKILL.md](skills/project-atlas-analyzer-skill/SKILL.md) |
| [`requirement-atlas-analyzer-skill`](skills/requirement-atlas-analyzer-skill/) | `requirement-atlas-analyzer` | 针对**一条**需求，梳理与现有代码的关系简报（主路径 · 分支 · 边界） | [README](skills/requirement-atlas-analyzer-skill/README.md) · [SKILL.md](skills/requirement-atlas-analyzer-skill/SKILL.md) |

补充材料（随子目录附带）：

- `harness-guide-generator-skill/examples/` — 指南生成示例  
- `project-atlas-analyzer-skill/reference.md`、`requirement-atlas-analyzer-skill/reference.md` — 证据路径与审阅要点  

---

## 🚀 怎么用

1. **获取本仓库**  
   克隆或下载到本地，确保你能看到 `skills/` 与各子目录。

2. **在 Cursor 里挂载 Skill**  
   将**需要的那一个**子目录（例如 `skills/harness-engineering`）配置为 Skill：放到个人目录 `~/.cursor/skills/<目录名>/`，或当前项目的 `.cursor/skills/<目录名>/`（以你使用的 Cursor 版本文档为准）。

3. **在对话里调用**  
   使用 `@` 引用该 skill 目录，或按各 `SKILL.md` 顶部的 `description` 所描述的场景自然触发；执行规则以对应目录下的 **`SKILL.md`** 为准。

4. **图谱类 Skill 的工作区**  
   使用 `repository-atlas` 或 `requirement-atlas-analyzer` 时，请在**要被分析的项目**中打开工作区，再 `@` 对应 skill；产出路径以各 `SKILL.md` 正文为准。

---

## 🎯 怎么选 Skill（速查）

| 你想…… | 优先用 |
|--------|--------|
| 对齐 Agent 架构、工具治理、安全与验证 | `harness-engineering` |
| 把一句需求变成「步骤 + 验收」的可粘贴指南 | `vibe-coding-harness-guide-generator` |
| 大项目拆版本、定里程碑与技术栈 | `large-project-versioned-roadmap` |
| 刚进仓，想先有一份与需求无关的仓库总览 | `repository-atlas` |
| 已有一条具体需求，想看清改哪里、边界在哪 | `requirement-atlas-analyzer` |

---

## 🔗 本仓库

- 主页：<https://github.com/RonnyJung2021/harness-engineering-skill>

---

<p align="center">
  <sub>🧩 Made for Cursor · 方法论在 Skill，落地在仓库</sub>
</p>
