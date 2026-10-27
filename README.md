# Research Experiment Skills

面向科研实验工作的 18 个 AI 技能，精选自 [Matt Pocock 的 skills 合集](https://github.com/mattpocock/skills)，并包含本地维护调整。

本仓库提供的是工作流程和指令；资料调查技能不等于完整的实验设计、统计审稿或论文评审体系。

## 技能目录

| Skill | 用途 |
| --- | --- |
| [code-review](skills/code-review/SKILL.md) | 检查代码规范，以及实现是否符合需求、实验计划和协议。 |
| [codebase-design](skills/codebase-design/SKILL.md) | 设计职责清楚、接口简单的代码模块。 |
| [diagnosing-bugs](skills/diagnosing-bugs/SKILL.md) | 系统定位运行错误、性能退化和异常输出。 |
| [domain-modeling](skills/domain-modeling/SKILL.md) | 统一研究概念、指标定义和决策记录。 |
| [grill-me](skills/grill-me/SKILL.md) | 通过追问检验想法与方案的通用入口。 |
| [grill-with-docs](skills/grill-with-docs/SKILL.md) | 澄清方案，并维护术语表和重要决策记录。 |
| [grilling](skills/grilling/SKILL.md) | 深入追问研究问题、假设、变量和边界。 |
| [handoff](skills/handoff/SKILL.md) | 整理上下文、进展和下一步，供新会话接手。 |
| [improve-codebase-architecture](skills/improve-codebase-architecture/SKILL.md) | 扫描代码结构，生成可视化改进建议。 |
| [prototype](skills/prototype/SKILL.md) | 制作临时原型，验证交互、状态或逻辑设计。 |
| [research](skills/research/SKILL.md) | 调查可信一手资料，保存带来源的研究笔记。 |
| [retro](skills/retro/SKILL.md) | 复盘工作过程，改进工具、检查和代理环境。 |
| [tdd](skills/tdd/SKILL.md) | 先写测试，再实现和重构，验证关键逻辑。 |
| [teach](skills/teach/SKILL.md) | 在工作区中持续讲解与练习知识和技能。 |
| [to-questionnaire](skills/to-questionnaire/SKILL.md) | 整理需要导师或合作者回答的问题。 |
| [wait-what](skills/wait-what/SKILL.md) | 补齐背景，重新解释未理解的内容。 |
| [writing-for-agents](skills/writing-for-agents/SKILL.md) | 编写适合 AI 阅读与执行的指令和文档。 |
| [writing-fragments](skills/writing-fragments/SKILL.md) | 收集零散研究观察、想法和写作素材。 |

## 安装

将需要的技能目录从 `skills/` 复制到 `~/.codex/skills/`，每个技能保持独立目录及其支持文件。目标位置已有同名技能时，先比较差异，再决定是否覆盖。

技能是否支持自动触发或仅显式调用，以各自的 `SKILL.md` 和 `agents/openai.yaml` 为准。使用前阅读技能说明；运行环境、项目规则与用户授权仍然适用。

## 本地维护

- `code-review`：直接从用户要求、当前 README、实验计划和研究协议查找审查依据，移除对已删除初始化技能的依赖。
- `handoff`：推荐后续技能前检查当前目录及可用技能，缺少适用技能时直接描述下一步。
- `writing-fragments`：素材收集独立工作，后续成文由用户提出，不依赖其他写作技能。

`grill-me` 依赖 `grilling`；`grill-with-docs` 使用 `grilling` 与 `domain-modeling`。复制部分技能时，请一并检查其引用的其他技能。

## 来源与许可

上游项目：[mattpocock/skills](https://github.com/mattpocock/skills)。原作者 Matt Pocock；遵循仓库内的 [MIT License](LICENSE)。本仓库是个人筛选与维护的快照，不是上游官方发行版。

快照日期：2026-10-27（Asia/Shanghai）。文件内容来自本机当前保留的 18 个技能，未以最新上游版本覆盖。上游原始导入的精确提交未知；`provenance.json` 中的提交仅用于核对许可证来源。

`manifest.json` 记录各文件的 SHA-256。实验数据、模型、运行结果、账号配置与凭证不在此快照内。
