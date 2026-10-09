# PM Decision OS

一套面向真实产品决策与 AI Agent 落地的 Skills。

它不是文档生成器，而是一条完整的产品闭环：先确认事实与需求，再做决策、PRD、评审、数据、实验、原型和 Agent 方案，并且始终保留证据边界与验收标准。

## 工作方式

```text
事实分层 -> 需求体检 -> 产品决策 -> PRD/Agent 方案
    ^                               |
    |                               v
复盘迭代 <- 数据/实验/Badcase <- 评审与灰度上线
```

## Skills

| Skill | 解决的问题 |
|---|---|
| `pm-command-center` | 复杂任务分诊与 Skill 编排 |
| `pm-evidence-ledger` | 事实分层、版本判断与证据冲突 |
| `pm-requirement-triage` | 写 PRD 前的需求体检与优先级 |
| `pm-prd-delivery` | 可评审、可研发、可验收的 PRD |
| `pm-review-gate` | 跨角色评审与 GO/NO-GO |
| `pm-data-contract` | 指标、埋点、SQL 与数据验收 |
| `pm-experiment-plan` | A/B、灰度、护栏与止损 |
| `pm-decision-brief` | 一屏式业务决策简报 |
| `pm-prototype-acceptance` | 可运行原型与验收清单 |
| `pm-agent-blueprint` | Agent 工作流、工具、知识与评测 |

## 设计原则

- 线上与可执行证据优先于静态材料。
- 正式规则、历史规则、方案候选和分析推断必须分开。
- “功能做完”不等于“业务结果成立”。
- 主文讲业务规则，复杂公式和技术细节进入相邻附录。
- 数据必须写清粒度、去重、时区、归因和验证状态。
- 高影响 Agent 动作必须有人类确认、审计和回滚。
- 最小交付必须能被真实运行或验收。

## 安装

复制需要的 Skill 文件夹到 Agent 运行环境的技能目录。

Codex：

```bash
cp -R pm-agent-blueprint ~/.codex/skills/
```

Claude Code：

```bash
cp -R pm-agent-blueprint ~/.claude/skills/
```

## 示例

- “先判断这个需求有没有必要做，再决定要不要写 PRD。”
- “这个规则在会议、需求文档和线上配置里不一致，先帮我确认事实层级。”
- “给我一份可直接评审的需求，补齐异常、埋点、灰度和回滚。”
- “把这个客服流程设计成 Agent，明确工具、知识库、人机确认和评测。”
- “把这份分析压缩成老板能直接看的数据结论、功能动作和验证指标。”

## English Summary

PM Decision OS is a clean-room skill collection for evidence-led product decisions and controlled AI Agent delivery. It covers evidence classification, requirement triage, PRDs, review gates, analytics contracts, experiments, prototypes, executive briefs, and Agent blueprints.

## License

MIT License. See [LICENSE](LICENSE).
