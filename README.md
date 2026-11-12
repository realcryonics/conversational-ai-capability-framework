# Conversational AI Capability Framework (LV0–LV6)

**Status: V0.1 research draft — not a validated benchmark.**

A proposed **capability-oriented taxonomy** for open-ended human–AI conversations. It describes seven kinds of conversational tasks (LV0–LV6) by the **AI capabilities required to respond appropriately**, rather than ranking users or claiming that human needs naturally fall into seven levels.

## Research question

Different conversational situations call for different AI capabilities. Can we make these requirements explicit, evaluate them in controlled contexts, and identify mismatches between an AI response and a user's current conversational goal?

## Framework at a glance

| Level | Scenario | Main capability focus |
|---|---|---|
| LV0 | Information Retrieval / 信息获取 | Knowledge and factual accuracy |
| LV1 | Conversation / 闲聊 | Natural conversation and context handling |
| LV2 | Emotional Support / 情绪支持 | Emotion understanding and safe support |
| LV3 | Self Understanding / 自我理解 | User modeling and guided reflection |
| LV4 | Decision Support / 决策支持 | Decision reasoning and trade-offs |
| LV5 | Relationship Intelligence / 关系建立 | Long-term memory and relational continuity |
| LV6 | Identity Co-construction / 身份共建 | Identity understanding and future modeling |

**Read first:** [Level definitions](taxonomy/levels.md) · [Eight-dimensional matrix](taxonomy/capability_matrix.md) · [Evaluation protocol draft](evaluation/protocol.md) · [Research limitations](research/limitations.md)

## How to interpret the levels

- Levels describe **different task capability profiles**, not a measured general intelligence score.
- Higher LV does **not** imply a model is better on every dimension; the original matrix is non-monotonic (e.g., the knowledge requirement for LV0 exceeds that of LV6).
- A single dialogue can combine several goals; classification is context-dependent.
- Star ratings represent **proposed importance/requirement intensity**, not measured model performance.
- The original 'intervention depth' percentages are unvalidated conceptual annotations; see limitations.

## Repository contents

- `taxonomy/levels.md` — source-grounded definitions from the original framework table.
- `taxonomy/capability_matrix.md` + `taxonomy/capability_matrix.csv` — eight capabilities and proposed star requirements.
- `taxonomy/design_rationale.md` — provisional classification logic and open questions.
- `evaluation/protocol.md` — draft evaluation procedure and controls.
- `evaluation/annotation_template.csv` — an empty annotation schema (no product/user data).
- `examples/synthetic_scenarios.md` — newly written illustrative examples, not actual benchmark samples.
- `research/limitations.md` and `ROADMAP.md` — validation plan.

## What is not included

No proprietary character replies, internal prompts, product metrics, real user conversations, or source workbook are included. This draft includes only the framework abstraction. **Publication rights and potential employment-related IP obligations still require review before making a repository public or applying an open-source license.**

## License

No open-source license has been assigned pending ownership/permission verification. This repository should remain private until that review is complete.
