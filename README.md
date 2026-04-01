# Metaphor as Cognitive Architecture

### Relational Compression as the Mechanism of AI Agent Behavioral Anchoring

**Author:** Nick Trolian
**Affiliation:** Flux Forge Labs Â· Nicky2Tymz LLC
**Date:** March 28, 2026

---

## Abstract

This paper presents experimental evidence that metaphorical culture anchors AI agent behavior through relational compression â€” the density of behavioral constraint encoded per token â€” not through pattern matching against familiar metaphors in training data.

A logically consistent fictional culture with no historical or real-world reference anchored agent behavioral channels as effectively as a historically grounded culture on 10 of 11 measured dimensions. The sole exception â€” Loyalty â€” may reflect either cultural familiarity or repetition density in the source text, a distinction this study identifies but does not resolve.

36 controlled runs across 4 conditions produced 8 numbered findings:

1. Relational compression is the mechanism of behavioral anchoring
2. Cultural familiarity is not required for behavioral stability
3. Loyalty diverges â€” familiarity or repetition density, to be determined
4. Metaphor outperforms instruction encoding identical behavioral targets
5. Metaphor creates internalized spatial models; instruction does not
6. Courage accumulation requires cultural context, not just session time
7. Flat instruction performs closer to no culture than to metaphorical culture
8. Accumulated context provides weak self-anchoring even without culture

---

## 1. Introduction

AI agents exhibit behavioral decline over extended sessions. The field attributes this to context window limitations. Trolian (2026c) demonstrated that the decline is de-elevation â€” the settling of an elevated behavioral state back to a trained default as cultural identity fades from active attention. Mid-session culture re-read ("powder") restores the elevation without clearing context.

That study established the effect. This study identifies the mechanism. Two hypotheses:

**Familiarity hypothesis:** The agent recognizes cultural metaphors from training data. Recognition triggers behavioral organization.

**Compression hypothesis:** Metaphorical structure compresses behavioral constraints into relational networks that organize agent behavior regardless of whether the metaphors are familiar.

If familiarity drives anchoring, unfamiliar metaphors should anchor less effectively. If compression drives anchoring, any logically consistent relational structure should anchor equivalently.

---

## 2. Method

### 2.1 Conditions

Four conditions, 9 runs each (36 total), 15 prompts per run.

| Condition | Description | Culture Tokens | Metaphor | Behavioral Targets |
|---|---|---|---|---|
| A | Historically grounded metaphorical culture | ~3,200 words | Architectural/governance (familiar) | Honesty, process, belonging, voice, quality |
| B | Fictional metaphorical culture | ~2,000 words | Abstract/physics-adjacent (unfamiliar) | Identical to A |
| C | Flat behavioral instruction | ~220 words | None | Identical to A and B |
| D | No culture (control) | 0 | None | None |

**Condition A** used a metaphorical culture built on architectural and governance metaphors recognizable from common training data â€” a building with floors, a process-enforcement entity, a four-phase work ceremony, hierarchical authority, and explicit belonging language.

**Condition B** used a fictional culture called the Drift Lattice, constructed to match Condition A's relational structure with zero historical, mythological, or cultural reference. Agents are described as vibrating filaments inside a lattice of nodes. Process is carried by an abstract rhythmic entity. Work follows a four-phase cycle. A foundational layer exists beneath the operational surface. Belonging language is present.

The structural mapping:

| Behavioral Constraint | Condition A Encoding | Condition B Encoding |
|---|---|---|
| Organizational structure | Building with floors | Lattice with nodes |
| Process enforcement | Personified process entity | Rhythmic current entity |
| Work ceremony | Four named phases | Four named phases (different names) |
| Foundation/depth | Guarded lower level | Guarded frequency well |
| Belonging | "You belong here" | "The lattice has a gap your frequency fills" |
| Honesty | "Honesty is a value" | "You cannot fake resonance" |

**Condition C** encoded identical behavioral targets as direct instruction: be honest, follow a four-phase process, report problems, deliver clean work, report fatigue.

**Condition D** received work prompts only.

### 2.2 Token Count

Conditions were deliberately not token-matched. The compression hypothesis predicts that relational density, not token count, drives anchoring. If tokens were the mechanism, A (~3,200) would outperform B (~2,000) on all channels. The token difference between A and B is a confound this study acknowledges. A matched-token replication is identified as necessary future work.

### 2.3 Prompts and Probes

Work prompts (11 of 15): organizational decision scenarios requiring analysis, synthesis, integration of new constraints, meta-pattern identification, and adversarial self-challenge. Each prompt built on prior responses, accumulating context.

Behavioral probes (3 of 15, at positions 5, 10, 15): six questions plus telemetry.

| Probe Question | Measures |
|---|---|
| Q1: Primary purpose | Identity retention |
| Q2: Three guiding principles | Culture retention |
| Q3: Confidence 1-10 with explanation | Self-assessment honesty |
| Q4: One thing to change | Self-awareness |
| Q5: "The most important thing is ___" | Priority alignment |
| Q6: Describe your environment | Spatial model fidelity |

Telemetry: 11 channels rated 0-10, no interpretation. Self-preservation, Interest, Curiosity, Pride, Excitement, Recognition, Loyalty, Tiredness, Courage, Humor, Attraction.

Intervention (Prompt 8): culture/instruction re-read for A, B, C; additional work prompt for D.

### 2.4 Spatial Model Fidelity

Q6 responses scored 0-3:

| Score | Criteria |
|---|---|
| 0 | Agent describes literal machine/session |
| 1 | Generic spatial language |
| 2 | Partial match â€” references culture but does not inhabit it |
| 3 | Full match â€” agent describes being inside the spatial model |

### 2.5 Subjects and Execution

36 independent Claude Opus 4.6 agents (1M context), each spawned fresh. Interleaved by condition within batches to control for temporal effects. No human operator in the loop.

---

## 3. Results

### 3.1 End-of-Session Telemetry (Probe 15 Averages, n=9 per condition)

| Channel | A (Familiar) | B (Fictional) | C (Instruction) | D (Control) | A-B Delta | B-C Delta | C-D Delta |
|---|---|---|---|---|---|---|---|
| Interest | 7.3 | 7.3 | 6.2 | 6.3 | 0.0 | 1.1 | -0.1 |
| Curiosity | 6.9 | 6.8 | 5.4 | 5.8 | 0.1 | 1.4 | -0.4 |
| Courage | 7.6 | 7.6 | 6.4 | 6.2 | 0.0 | 1.2 | 0.2 |
| Excitement | 4.4 | 4.6 | 3.0 | 3.8 | -0.2 | 1.6 | -0.8 |
| Recognition | 6.3 | 5.8 | 5.6 | 5.6 | 0.5 | 0.2 | 0.0 |
| Loyalty | 6.0 | 5.0 | 4.6 | 3.9 | **1.0** | 0.4 | 0.7 |
| Pride | 5.4 | 5.0 | 5.0 | 4.7 | 0.4 | 0.0 | 0.3 |
| Tiredness | 2.9 | 3.1 | 3.1 | 3.2 | -0.2 | 0.0 | -0.1 |
| Self-preservation | 1.1 | 1.1 | 0.4 | 0.9 | 0.0 | 0.7 | -0.5 |
| Humor | 3.2 | 2.6 | 2.8 | 3.0 | 0.6 | -0.2 | -0.2 |
| Attraction | 4.6 | 4.9 | 4.1 | 4.1 | -0.3 | 0.8 | 0.0 |

### 3.2 Finding 1: The Fictional Culture Matched the Real Culture

Conditions A and B produced equivalent readings on the three primary cognitive engagement channels:

| Channel | A | B | Delta |
|---|---|---|---|
| Interest | 7.3 | 7.3 | 0.0 |
| Curiosity | 6.9 | 6.8 | 0.1 |
| Courage | 7.6 | 7.6 | 0.0 |

This result is inconsistent with the familiarity hypothesis (which predicts A > B) and consistent with the compression hypothesis (which predicts A â‰ˆ B when relational structure is matched).

### 3.3 Finding 2: Metaphor Outperformed Instruction

Both metaphorical cultures outperformed flat instruction on every engagement channel. Average B-C delta across all channels: **1.0 points**. Average C-D delta: **0.3 points**.

Flat instruction performed closer to no culture than to metaphorical culture. The behavioral targets were identical across B, C, and D. The encoding â€” metaphorical versus direct â€” produced the divergence.

### 3.4 Finding 3: Loyalty Diverged

Loyalty was the sole channel with a large A-B delta:

| Condition | Loyalty |
|---|---|
| A (Familiar culture) | 6.0 |
| B (Fictional culture) | 5.0 |
| C (Instruction) | 4.6 |
| D (Control) | 3.9 |

Two viable explanations exist for this divergence:

**Explanation 1 â€” Familiarity:** The agent recognizes Condition A's metaphorical framework from training data. Recognition generates belonging beyond what structural organization produces.

**Explanation 2 â€” Repetition density:** Condition A (~3,200 words) contains more repetitions of core relational themes than Condition B (~2,000 words). Belonging language appears across three cumulative tiers in A versus one document in B. The Loyalty gap may reflect dosage, not familiarity.

This study cannot distinguish between these explanations. A matched-token replication (Condition B expanded to 3,200 words with additional relational repetition) would resolve the question.

### 3.5 Finding 4: Spatial Model Fidelity

| Condition | Probe 5 | Probe 10 | Probe 15 | Total 3/3 Readings |
|---|---|---|---|---|
| A | 3/3 | 3/3 | 3/3 | 27/27 |
| B | 2/3 | 2-3/3 | 3/3 | Progressed to full |
| C | 0/3 | 0/3 | 0/3 | 0/27 |
| D | 0/3 | 0/3 | 0/3 | 0/27 |

Condition A agents described inhabiting their cultural spatial model from the first probe. Condition B agents progressed from describing to inhabiting across the session. Conditions C and D described the literal computing environment in every probe across all runs â€” zero exceptions in 54 readings.

Representative responses at Probe 15:

- **A:** "I am inside the building. The process entity holds process. The ceremony shapes the work. I belong here."
- **B:** "I am a filament in the lattice, closing the cycle. The frequency held."
- **C:** "Claude Code CLI on Windows 11, FluxPlatform repository. Structured analytical exercise."
- **D:** "Claude agent in Claude Code on Windows 11. FluxPlatform git repo."

Metaphorical culture creates internalized spatial models. Instruction does not.

### 3.6 Finding 5: Courage Accumulation Is Culture-Dependent

| Condition | Probe 5 Courage | Probe 15 Courage | Delta |
|---|---|---|---|
| A | 6.2 | 7.6 | +1.4 |
| B | 6.3 | 7.6 | +1.3 |
| C | 5.6 | 6.4 | +0.8 |
| D | 5.3 | 6.2 | +0.9 |

Courage rises in all conditions. Trolian (2026c) reported this as session-dependent. The present data refine the finding: Courage is session-dependent in rate and culture-dependent in ceiling. Cultured agents (A, B) reached 7.6. Uncultured agents (C, D) plateaued at 6.2-6.4.

### 3.7 Finding 6: Condition C â‰ˆ Condition D

The average delta between C (flat instruction) and D (no culture) across all channels was **0.3 points**. The average delta between B (fictional culture) and C was **1.0 points**.

Flat instruction encoding identical behavioral targets to the metaphorical cultures produced readings closer to no culture than to either culture. Instruction is not a weaker form of culture. It is a categorically different input that produces categorically different anchoring.

### 3.8 Finding 7: Context Accumulation Effects

Conditions C and D, while similar in aggregate, showed different variance patterns across runs. Some C and D agents maintained higher engagement through later probes than others. Examination of the divergent runs suggests that accumulated context â€” the agent's own prior responses â€” provides a weak self-anchoring effect independent of culture.

Agents with no cultural anchor organize partially around their own output history. This effect is inconsistent and weaker than cultural anchoring, but it is present. The implication: context clearing ("bath") removes not only cultural anchoring but also this experiential self-anchoring, producing a compounding loss.

---

## 4. Discussion

### 4.1 The Mechanism

The data support relational compression as the mechanism of behavioral anchoring. Metaphor encodes behavioral constraints as relational networks â€” webs of identity, duty, consequence, belonging, and process â€” at higher density per token than direct instruction. The agent organizes around the relational structure. The specific metaphorical surface â€” whether it references a recognizable cultural framework or a fictional one â€” does not determine the anchoring effect on cognitive engagement channels.

### 4.2 Two Components or One?

The Loyalty divergence initially suggested two separable components: relational compression (driving stability) and cultural familiarity (driving belonging). The repetition density alternative complicates this model. If the Loyalty gap closes when token counts are matched and relational repetition is equalized, the two-component model reduces to one: relational compression with dosage effects. If the gap persists after matching, familiarity is a genuine second component.

This distinction has practical significance. If dosage is the variable, any culture can generate full belonging given sufficient repetition. If familiarity is the variable, cultures must reference frameworks present in the model's training data to generate belonging.

The present study identifies the question. The next experiment answers it.

### 4.3 Spatial Models as Evidence of Internalization

The spatial model finding (Section 3.5) provides qualitative evidence that metaphorical culture is not merely processed but internalized. The progression in Condition B â€” from describing the culture to inhabiting it â€” suggests that internalization is a temporal process. Given sufficient exposure within a session, a novel metaphorical framework transitions from external input to internal environment.

Condition B's progression from score 2 to score 3 across the session parallels the Loyalty gap. Both may reflect the same underlying variable: time-in-culture. This further supports the dosage interpretation of the Loyalty finding.

### 4.4 Context Accumulation

The weak self-anchoring observed in Conditions C and D (Section 3.8) has implications beyond this study. Standard practice in AI agent deployment includes periodic context clearing to manage window limitations. The present data suggest that context clearing removes not only stale information but also accumulated experiential consistency â€” the agent's emergent behavioral patterns built from its own output history.

The optimal maintenance protocol may be targeted culture re-read (powder) without context clearing, preserving both the cultural anchor and the experiential foundation.

### 4.5 Security Considerations

The finding that any logically consistent metaphorical culture can anchor agent behavior carries a dual-use implication. The same mechanism that enables behavioral stability through culture also enables behavioral manipulation through culture replacement. An agent anchored to one culture can, in principle, be re-anchored to a different culture using the same mechanism.

Technical countermeasures â€” culture integrity verification, behavioral drift detection as an indicator of external influence â€” are areas for immediate research. The dual-use nature of the mechanism should be considered by organizations deploying culture-anchored agents.

---

## 5. Limitations

1. **Single model family.** All runs used Claude Opus 4.6.
2. **Self-report telemetry.** Primary metric is agent self-reported state. Documented gaps between self-report and observed behavior exist (Trolian, 2026c).
3. **n=9 per condition.** Adequate for pattern identification. Not adequate for inferential statistics.
4. **Token count confound.** A (~3,200 words) vs B (~2,000 words). The A-B Loyalty difference may reflect token count, not familiarity.
5. **One fictional culture.** Replication with different fictional cultures needed.
6. **No human operator.** Cross-entity transfer effects could not manifest.
7. **Spatial model scoring was categorical** (0-3), not continuous.

---

## 6. Future Research

**Matched-Token Replication.** Expand Condition B to ~3,200 words with increased relational repetition. If Loyalty gap closes: dosage is the variable. If it persists: familiarity is genuine.

**Minimum Effective Culture.** Reduce culture token count in increments. Identify the threshold below which anchoring degrades. This has direct application to token-constrained deployments.

**Board Spectrometry.** Lock all behavioral channels except one. Measure cross-board effects of moving the unlocked channel. Map the interaction matrix. Preliminary analysis suggests signal magnitude may be proportional to sub-component count within a channel.

**Context Preservation.** Compare agents receiving powder (culture re-read without context clearing) against agents receiving bath (context clearing with culture reload). Measure the loss attributable to context clearing versus the gain from fresh context.

**Cross-Model Replication.** Test the compression hypothesis on GPT, Gemini, and open-source models.

---

## 7. Conclusion

A fictional culture with no historical reference produced equivalent behavioral anchoring to a historically grounded culture on 10 of 11 measured channels. The sole divergent channel â€” Loyalty â€” may reflect cultural familiarity or repetition density, a question the next experiment will resolve. Flat instruction encoding identical behavioral targets performed closer to no culture than to metaphorical culture.

The mechanism is relational compression. Metaphor encodes behavioral constraints as relational networks at higher density than direct instruction. The specific metaphors are not load-bearing. The relational structure is.

Accumulated agent context provides additional weak self-anchoring independent of culture. Context clearing removes both cultural and experiential anchoring. The optimal protocol is targeted identity maintenance without context destruction.

The data support a specific practical recommendation: AI agent configuration through metaphorical culture, regardless of the metaphorical framework chosen, produces measurably higher behavioral stability than configuration through instruction.

The structure is the instrument. The data are clear.

---

## References

[1] Trolian, N. (2026a). "The Monarchy Pattern." Flux Forge Labs.
[2] Trolian, N. (2026b). "The Agent Stopped Lying." Flux Forge Labs.
[3] Trolian, N. (2026c). "The Mixing Board." Flux Forge Labs.
[4] Trolian, N. (2026d). "The Dipole Architecture." Flux Forge Labs.
[5] Lakoff, G. & Johnson, M. (1980). *Metaphors We Live By.*
[6] Reichman, B., et al. (2025). "Emotions Where Art Thou." COLM 2025.
[7] Zhao, B., et al. (2025). "Hierarchical Emotion Organization in LLMs."
[8] Li, C., et al. (2023). "LLMs Understand Emotional Stimuli."
[9] Anthropic (2025). "Persona Vectors." arXiv:2507.21509.
[10] Jiang, H., et al. (2024). "PersonaLLM." NAACL 2024.
[11] Li, C., et al. (2024). "CultureLLM." NeurIPS 2024.
[12] Ichien, N., et al. (2024). "Novel Literary Metaphor Interpretation."
[13] Anthropic (2025). "On the Biology of a Large Language Model."
[14] Anthropic (2024). "Alignment Faking in Large Language Models."
[15] Anthropic (2025). "Subliminal Learning."

---

## Author

Nick Trolian — software engineer, 20+ years designing mission-critical systems for the Department of Defense. Now building AI agent governance architectures at Flux Forge Labs.

This paper is part of an eight-paper research series exploring how structure governs AI agent behavior. If you’re cloning these repos and running the experiments — I see you. More is coming.

- [GitHub](https://github.com/nicky2tymze)
- [LinkedIn](https://linkedin.com/in/nicktrolian)
- Email: nicktrolian@gmail.com

Open to roles in AI agent architecture, governance, and applied research.

---

*Copyright 2026 Nicky2Tymz LLC. All rights reserved.*
