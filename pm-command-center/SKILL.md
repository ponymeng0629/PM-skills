---
name: pm-command-center
description: 负责复杂产品任务的分诊、证据检查、Skill 路由与交接。适用于用户只有一个模糊目标，或任务同时涉及需求、PRD、数据、实验、评审、原型及 Agent 方案时。
---

# PM Command Center

把模糊任务转成一条最短、可验证的产品工作链路。不要默认调用全部 Skill。

## 第一步 识别任务所处阶段

判断当前需要的是：发现问题、确认规则、做决策、写需求、评审、验证数据、设计实验、做原型，还是设计 Agent。

同时写清：

- 谁在做决定，谁受影响；
- 当前必须回答的一个核心问题；
- 已有证据、缺失证据和时间边界；
- 哪些外部动作尚未得到授权。

## 第二步 选择最小 Skill 组合

| 任务 | 使用 Skill |
|---|---|
| 材料相互冲突或状态不清 | `pm-evidence-ledger` |
| 需求模糊、价值不清、边界不清 | `pm-requirement-triage` |
| 需要可评审、可研发、可验收的需求 | `pm-prd-delivery` |
| 需要多角色评审与 GO NO-GO | `pm-review-gate` |
| 指标、埋点、SQL 或口径不清 | `pm-data-contract` |
| 需要 A/B、灰度或因果验证 | `pm-experiment-plan` |
| 需要给老板或跨部门快速汇报 | `pm-decision-brief` |
| 需要从截图、描述产出交互原型 | `pm-prototype-acceptance` |
| 需要设计可落地的 Agent | `pm-agent-blueprint` |

## 交接摘要

每个环节结束时只交接六项：已确认事实、已做决策、未决问题、交付物、下一步、停止条件。

## 完成标准

输出当前结论、选择的 Skill 链路、必要输入、责任人和验证指标。若继续推进需要新证据或新授权，明确停下，不用推测补齐。
