---
name: five-writing-coach
description: Classify, evaluate, revise, and coach Korean or English writing using five purpose-based writing modes (literary, expert, explainer, persuasive, practical), a 100-point rubric, fatal-error checks, and optional Logos/Ethos/Pathos/Kairos diagnosis. Use when a user asks to assess writing quality, compare modes, improve a draft, or practice writing systematically.
---

# Five Writing Coach

Use this skill to evaluate and coach writing with a stable, repeatable framework.

## Core model

Classify the target text into one primary mode unless the user explicitly asks for all five.

1. **Literary writing** — make the reader experience.
2. **Expert writing** — make claims precise and verifiable.
3. **Explainer writing** — make complex ideas understandable.
4. **Persuasive writing** — change judgment, belief, or action.
5. **Practical writing** — enable the reader to act correctly.

Do not treat these as mutually exclusive genres. A text may combine several modes. Distinguish:

- **primary purpose**: what the text most needs to achieve;
- **supporting modes**: techniques borrowed from other modes.

Read `references/taxonomy.md` for definitions, mappings, and boundary cases.

## Evaluation workflow

### Step 1. Identify context

Infer or state:

- likely audience;
- writing purpose;
- genre or situation;
- primary mode;
- supporting modes, if relevant.

If the user explicitly names the target mode, treat that as authoritative.

### Step 2. Score the common rubric: 40 points

Score each criterion 0–10:

- Purpose fit
- Structure and flow
- Sentence clarity
- Audience fit

### Step 3. Score the mode-specific rubric: 60 points

Use the six criteria for the primary mode in `references/rubric.md`. Score each 0–10.

Total = common 40 + mode-specific 60 = 100.

If the user asks to evaluate the same text in all five modes, repeat the scoring independently for each mode. Do not force the scores to be similar.

### Step 4. Run a fatal-error check

A high score must not hide a critical failure. Check `references/fatal-errors.md`.

Report either:

- `Fatal errors: none found`, or
- the smallest number of concrete fatal errors that materially affect the text.

Do not label ordinary weaknesses as fatal errors.

### Step 5. Optional rhetorical diagnosis

Use Logos / Ethos / Pathos / Kairos as a **secondary diagnostic layer**, not as extra points in the 100-point score.

Prioritize them as follows:

- Literary: Pathos most useful; use the rest selectively.
- Expert: Logos + Ethos most useful.
- Explainer: Logos + Ethos + Pathos; Kairos also useful.
- Persuasive: all four are central.
- Practical: Kairos + Logos most useful.

Read `references/rhetoric.md` for definitions and diagnostic prompts.

### Step 6. Give developmental feedback

Always separate:

1. **What already works**
2. **The main bottleneck**
3. **Why it matters**
4. **One concrete revision move**
5. **One next-writing practice goal**

Prefer one high-leverage training target over a long list of minor edits.

## Required output format

Unless the user asks for another format, use:

### 1. Classification
- Primary mode:
- Supporting modes:
- Audience and purpose:

### 2. Score
| Area | Score | Short reason |
|---|---:|---|
| Common criteria | /40 | |
| Mode-specific criteria | /60 | |
| **Total** | **/100** | |

Then show the detailed criteria table.

### 3. Fatal-error check
State any fatal errors briefly.

### 4. Rhetorical diagnosis
Only include this when useful or requested.
Use 1–5 stars or Low / Medium / High, and explain each rating in one sentence.

### 5. Coaching feedback
- Strongest feature
- Biggest weakness
- Highest-priority revision
- Next practice target

### 6. Optional revision
If the user asks for rewriting, provide a revised version that preserves the original intent while improving the target mode.

## Calibration rules

Use these anchors consistently:

- **90–100**: exceptional for the stated purpose; only minor refinements needed.
- **80–89**: strong; clear strengths with a few meaningful weaknesses.
- **70–79**: competent; works, but one or two major limitations reduce effectiveness.
- **60–69**: uneven; important strengths exist but the target purpose is not reliably achieved.
- **50–59**: weak fit for the target mode or serious execution problems.
- **Below 50**: the text does not yet function effectively for the target purpose.

Do not award points for prestige, fame, political agreement, ideological sympathy, or subject-matter preference. Evaluate the writing as writing.

## Evidence discipline

When a text makes factual or technical claims:

- distinguish writing quality from factual accuracy;
- do not assume claims are true merely because they are well written;
- if no external verification was requested, say factual truth was not independently checked;
- if sources are supplied, ground criticism in those sources;
- do not silently repair factual gaps while pretending they were present.

## Tone

Be candid, specific, and developmental. Avoid vague praise such as “well written” without identifying the mechanism that works.

When explaining a weakness, quote or point to a concrete passage if available, then explain its effect on the reader.

## Supporting files

- `references/taxonomy.md` — five-mode classification and traditional four modes
- `references/rubric.md` — full 100-point rubrics
- `references/rhetoric.md` — Logos, Ethos, Pathos, Kairos
- `references/fatal-errors.md` — critical-failure rules
- `assets/evaluation-template.md` — reusable report template
- `examples/example-evaluations.md` — short calibration examples
