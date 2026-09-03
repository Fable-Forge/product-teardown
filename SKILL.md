---
name: product-teardown
description: Use when the user asks for 产品拆解, 竞品分析, product teardown, why a product or game works, core loop, moat, retention, monetization, AI readiness, game mechanics, 叙事交互, reference-title lessons, or project-fit recommendations. Also use for 调研这个网站, 调研 X, 研究下 X, 看看这个网站/工具站/独立站/app, 说出你的想法, 总结提炼延伸, 这篇文章对我的项目有什么帮助, 复刻/仿做 X, or questions about 功能, 定位, 受众, 盈利模式, 订阅, 月访问量, 流量来源. Applies to products, games, external articles, and methodologies.
---

# Product Teardown

## Overview

Reverse-engineer a product or game as a system, then judge what is actually useful for the user's current project. Prefer mechanisms, decisions, loops, tradeoffs, and evidence over feature lists or admiration.

## Route the Request

- For SaaS, AI tools, apps, platforms, plugins, or workflows, read `references/product-mode.md`.
- For games, narrative experiences, interactive systems, or reference titles, read `references/game-mode.md`.
- For an external article, 公众号 post, or methodology (no product to inspect), skip mechanism reverse-engineering: extract the claim, the conditions it depends on, and the falsifying case, then go straight to step 5 project fit. The recurring ask is 对我的项目有什么帮助 as a 清单, not a summary.
- For a quick teardown, full report, or project-fit comparison, also read `references/output-templates.md`.
- For a screen or multi-step UX flow audit, use `product-design:audit` instead.
- For implementation, keep this skill's conclusion as design direction; invoke the relevant engine, frontend, or project skill for wiring and code.

## Workflow

1. Frame the decision.
   - Identify the target, analysis scope, and the decision the user needs to make.
   - Use quick depth for “值不值得看 / 简单拆一下”; use full depth for “深入 / 完整 / 调研”.
   - State assumptions when missing information does not block useful analysis. Ask one question only when different answers would materially change the conclusion.
   - 先查有没有研究过（去重）。开工前按域名、产品名或文章标题搜索用户可用的 Knowledge 区与会话日志；命中就先给出上次结论并只补增量，不要从头重做。若这些来源不存在，明确说明后继续。

2. Build an evidence ledger（证据账本）.
   - Inspect user-provided files, screenshots, URLs, or repositories first.
   - For current external claims, use `agent-reach` and prefer primary or authoritative sources.
   - For the user's own project, inspect its current source-of-truth docs and live runtime tree. Do not rely on stale project memory when current files are available.
   - Label material claims as `事实`, `来源`, `推断`, or `待补`; never invent users, revenue, retention, conversion, ratings, or technical capabilities.

3. Reverse-engineer the system.
   - Find the promise, user or player job, core entities, input-decision-feedback loop, retention or return driver, and business or production constraints.
   - Explain why each mechanism works, when it stops working, and what tradeoff makes it possible.
   - Separate category demand, distribution, brand, and timing from product quality.

4. Test the thesis adversarially.
   - Name the strongest alternative explanation for success.
   - Find the missing loop, weak audience fit, hidden cost, or production burden.
   - Distinguish visible surface treatment from the underlying mechanism worth borrowing.

5. Map to the user's project when requested.
   - Compare the reference against the project's audience, core loop, accepted baseline, team size, art/content budget, technical stack, and delivery stage.
   - Classify each idea as `保留`, `改造`, or `不采用` with a reason.
   - Separate `设计方向` from `实现/接线`; do not present implementation as complete unless the user requested and verified it.
   - Keep `待选` and `已采纳` distinct. Mark an idea adopted only after the user decides or the project's source-of-truth document is updated.

6. Deliver the smallest useful report.
   - Lead with a sharp verdict, then evidence and implications.
   - Default to Chinese when the request is Chinese.
   - Save Markdown or HTML only when requested, using the user's path or a path inside the current workspace. Never hardcode a personal desktop path or open a browser without permission.

## Quick Reference

| Request | Depth | Required references | Default ending |
|---|---|---|---|
| “这个产品值不值得学” | Quick | Product or game mode + output templates | 3-point project fit |
| “完整拆解 X” | Full | Product or game mode + output templates | Verdict + risks + opportunities |
| “X 对我的项目有什么用” | Full, scoped | Relevant mode + output templates | 保留 / 改造 / 不采用 |
| “照着 X 实现” | Teardown first | Relevant mode | Design direction, then implementation handoff |

## Example: Borrow the Mechanism, Not the Surface

Observation: a product's command palette makes repeated actions feel instant.

- Weak transfer: add the same shortcut UI to a narrative game because it looks polished.
- Strong transfer: identify the mechanism as reducing repeated-action latency, verify that the game has a repeated high-friction action, then choose a fitting control pattern for that platform and audience.

## Self-Check

- Is the verdict supported by evidence rather than taste?
- Did the analysis expose a loop and a tradeoff, not just features?
- Are inference and unknowns visible?
- Are recommendations specific to the target project's current constraints?
- Could the user act on the top recommendation as a bounded experiment?
