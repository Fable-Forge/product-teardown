# Output Templates

Choose the smallest template that answers the user's decision. Keep claims labeled and citations close to current external facts.

## Evidence Labels

- `事实`: directly observed in the product, game, repository, or supplied artifact.
- `来源`: supported by a cited current source.
- `推断`: reasoned conclusion from visible evidence.
- `待补`: important missing information that limits confidence.

## Quick Teardown

```markdown
# [Target] 快速拆解

## 一句话判断
[Useful conclusion, not a description]

## 它真正卖的是什么
[Promise, audience, and strategic bet]

## 核心循环
[Trigger -> decision/action -> feedback/value -> return]

## 为什么有效
1. [Mechanism + evidence]
2. [Mechanism + evidence]
3. [Mechanism + evidence]

## 最先出问题的地方
[Highest-impact weakness or hidden cost]

## 对当前项目的价值
- 保留：[Mechanism]
- 改造：[Mechanism and required adaptation]
- 不采用：[Surface or mechanism that does not fit]
```

## Full Teardown

```markdown
# [Target] 产品/游戏拆解

## 结论摘要
[Why it wins, where it breaks, what is hard to copy]

## 证据与假设
[Facts, sources, inferences, unknowns]

## 用户/玩家与核心承诺
[Audience, job/fantasy, trigger, context]

## 系统与核心循环
[Entities, state, decisions/actions, feedback, return]

## 体验与工艺
[Concrete patterns and tradeoffs]

## 增长/留存/进程
[Use concepts appropriate to product or game]

## 商业与市场
[Monetization, positioning, alternatives]

## 壁垒与竞争
[Temporary, operational, durable]

## 弱点与风险
| Risk | Evidence | Severity | Time horizon | Mitigation |
|---|---|---|---|---|

## 机会
[Bounded improvement, strategic shift, optional high-risk bet]

## 最终判断
[Decision-ready verdict]
```

## Project-Fit Memo

Use this when the user asks what an external reference means for an existing project.

```markdown
# [Reference] -> [Project] 适配判断

## 当前基线
[Current source-of-truth files, accepted loop, constraints]

## 适配矩阵
| Reference mechanism | Evidence | Fit | Decision | Smallest experiment | Cost/risk |
|---|---|---|---|---|---|
| [Mechanism] | [Fact/source] | High/Med/Low | 保留/改造/不采用 | [Bounded test] | [Burden] |

## 设计方向
[What should change in experience, rules, pacing, or content]

## 实现/接线
[What would need code, data, assets, tests, or migration; do not claim it is done]

## 状态
- 待选：[Ideas awaiting a decision]
- 已采纳：[Only user-approved or source-of-truth-synced decisions]
```

## Quality Gate

Before delivery, remove:

- feature-list summaries without a system thesis
- unsupported numerical claims
- generic advice that could apply to any product or game
- recommendations that ignore the current project's accepted baseline
- copied surface details with no explanation of the underlying mechanism
