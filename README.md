# claude-deconstruct

A Claude Code plugin for first-principles analysis. Surfaces hidden assumptions, establishes foundational truths, rebuilds the problem from scratch, and identifies the high-leverage move that conventional analysis would miss.

Modeled on Aristotle's method: find the truths that cannot be derived from anything more basic, then reason upward from those alone.

---

## What it does

You run `/deconstruct` and describe a problem, decision, or situation. The skill walks four phases:

1. **Surface the assumptions** — what's embedded in how you framed it (and which are load-bearing)
2. **Establish first principles** — what's true independent of convention or prior strategy
3. **Rebuild from the foundation** — three distinct approaches, optimized for speed, impact, simplicity
4. **The high-leverage move** — the single action that's invisible under conventional analysis

Two modes:
- **Fast** (Phase 1 + Phase 4) — for daily decisions, auto-triggers
- **Full** (all four phases) — for pricing, business models, career decisions, strategy pivots

The fear flag is built in: when an assumption traces back to fear, the skill names it and points to journaling instead of strategy. Fear-origin assumptions are rarely intellectual problems.

---

## Install

```bash
claude plugin add github.com/adelaidasofia/claude-deconstruct
```

Then in any Claude Code session:

```
/deconstruct
```

The skill will prompt for the problem you want to deconstruct.

---

## Requirements

- Claude Code
- Nothing else

**Optional integrations:**
- Decision template with `stakes: high` field — auto-offers fast mode on high-stakes entries (set `deconstruct_auto: true` in the decision frontmatter to enable)
- The daily-journal or insights plugin — adds a "first-principles audit" step to weekly review (flags high-stakes decisions made without a deconstruct pass)

---

## When to run it

This skill works best when you suspect you're stuck inside assumptions you can't see:

- A pricing model copied from competitors without questioning why
- A product roadmap built on what users say they want vs. what they actually need
- A career path followed because "that's how it's done in this industry"
- A business model that feels stuck but can't figure out why
- A hiring process, marketing strategy, or workflow everyone told you was "best practice"
- A competitive analysis where you're parroting positioning instead of finding your edge
- Any decision where "we've always done it this way" is the real answer

The full run is heavy. Don't run it on trivial decisions. Fast mode exists for a reason.

---

## What makes this different from "list pros and cons"

Pro/con lists assume the framing is correct. Deconstruction questions the framing.

Most decision tools take your problem statement as given and help you optimize within it. This skill assumes the problem statement itself is contaminated by convention, imitation, precedent, fear, and unexamined defaults — and forces you to strip those out before you reason about solutions.

The 3-question test in Phase 2 is the core. If a statement is only true because everyone else does it, it's not a first principle. It's a habit.

---

## Submitting to the Cowork marketplace

Once the repo is on GitHub, submit at: **[clau.de/plugin-directory-submission](https://clau.de/plugin-directory-submission)**

For the community marketplace:

```bash
claude plugin marketplace add anthropics/claude-plugins-community
```

---

## License

MIT
