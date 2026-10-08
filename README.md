# Five Writing Coach

A reusable writing-evaluation and coaching skill built around five purpose-driven writing modes.

## What it does

Five Writing Coach distinguishes five writing purposes:

1. **Literary** — make the reader experience.
2. **Expert** — make claims precise and verifiable.
3. **Explainer** — make complex ideas understandable.
4. **Persuasive** — change judgment, belief, or action.
5. **Practical** — enable correct action.

It evaluates writing with:

- a **40-point common rubric**;
- a **60-point mode-specific rubric**;
- a **fatal-error check**;
- optional **Logos / Ethos / Pathos / Kairos** diagnosis;
- one prioritized revision and one next-practice goal.

## Why this framework exists

Traditional writing instruction often distinguishes four discourse modes — **narration, description, exposition, and argumentation**. Those categories mainly describe *how a passage operates*.

This project adds a second layer: *what change should happen in the reader?*

The two systems are complementary:

- Four traditional modes = **methods**
- Five purpose-driven modes = **goals**

## Typical use cases

- “Evaluate this as explainer writing.”
- “Score this article in all five modes.”
- “Why is this persuasive but weak as expert writing?”
- “Revise this science article without losing accuracy.”
- “Diagnose Logos, Ethos, Pathos, and Kairos.”
- “Give me one training target for my next piece.”

## Common genre mappings

### Science journalism

Primarily **Explainer writing**:

> Explainer structure + Expert accuracy + Literary readability

### Argumentative columns

Primarily **Persuasive writing**:

> Persuasive argument + Expert evidence + Explainer clarity + optional Literary devices

## Repository structure

```text
five-writing-coach/
├── SKILL.md
├── README.md
├── README.ko.md
├── CHANGELOG.md
├── LICENSE
├── references/
│   ├── taxonomy.md
│   ├── rubric.md
│   ├── rhetoric.md
│   └── fatal-errors.md
├── assets/
│   └── evaluation-template.md
└── examples/
    └── example-evaluations.md
```

## Example prompt

```text
Use Five Writing Coach to evaluate the text below.
Target mode: Explainer writing.
Also diagnose Logos, Ethos, Pathos, and Kairos.
Give me one main weakness and one exercise for my next piece.

[TEXT]
```

## Scoring philosophy

A 90 in one mode does not imply a 90 in another.

A powerful argumentative essay may be a poor practical memo. A beautiful literary passage may be weak expert writing. Five Writing Coach therefore evaluates **fitness for purpose**, not generic “good writing.”

## Development principle

The framework is designed for deliberate practice:

1. declare the target mode;
2. score with the same rubric;
3. identify the main bottleneck;
4. revise one high-leverage weakness;
5. set one goal for the next piece;
6. repeat and compare over time.

## Version

Current public draft: **0.1.0**

## License

MIT. See [LICENSE](LICENSE).
