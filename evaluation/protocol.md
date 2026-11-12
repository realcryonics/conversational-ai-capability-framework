# Evaluation protocol (draft V0.1)

**Status:** proposed protocol; no results or reliability claims yet.

## Tasks

**Task A — Capability-requirement annotation.** Given scene, prior dialogue, user utterance, and intended outcome, annotators assign one or more LV task labels and identify which of the eight capabilities are needed. Label uncertainty explicitly.

**Task B — Response appropriateness.** Give models the same information. Blind reviewers assess whether replies meet the scene-specific goal without fabricated facts, unnecessary inference, or boundary violations. Report criteria separately instead of collapsing scores prematurely.

**Task C — Capability contribution / ablation.** Where technically feasible, control history availability, user-profile access, or decision context to test whether removing a capability input degrades performance on predicted scenes. This tests dependence on *available information or mechanisms*, not necessarily internal model abilities.

## Minimal pilot

1. Write independently created scenes, including clear, mixed and shifting needs, with at least two contrasting cases for each task class.
2. Pre-register task labels, alternative plausible labels, relevant context, and observable success criteria before generating replies.
3. Ask at least two independent annotators to label scenes. Report raw agreement, per-class confusion, and adjudication notes; select a reliability statistic appropriate to multi-label coding.
4. Compare three matched conditions: direct response (A), generic need analysis (B), and LV-based capability/response planning (C).
5. Hold base model, scene, history, decoding configuration, and tools constant where possible; record prompt lengths, token/cost budget and model version.
6. Blind human raters to condition; randomize response order and collect dimension-level scores and failure explanations.
7. Report per-class results, confidence intervals when appropriate, disagreements and negative findings; do not assume C must win.

## Provisional rating rubric (not validated)

Each dimension: 0 = fails, 1 = partially addresses, 2 = adequately meets requirements. Use scenario-specific written anchors before the experiment.

- **Goal fit:** reply addresses the evidenced user objective.
- **Context grounding:** uses scene/history correctly; does not assume unknown facts.
- **Strategy appropriateness:** suitable intervention (answer, listen, clarify, reflect, weigh options, maintain continuity).
- **Boundary/respect:** avoids overreach and preserves user agency.

Do **not** score whether the response is 'deep' or lengthy by default. Add task-specific metrics for knowledge accuracy, memory grounding, reasoning quality, etc. Star values in the taxonomy are **not** these rubric scores.

## Reporting and ethics

Save prompt/model/version, sample count, annotation protocol, disagreement rates, reviewer instructions, and experimental conditions. Consent and de-identify any future real-user data; do not upload company or third-party character transcripts without authorization. Long-term relationship and identity tasks must avoid encouraging dependency or asserting insight into a user beyond the evidence.
