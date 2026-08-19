---
name: neo-slow-media-lens
description: Apply xiaojiahaina's neo-slow media editorial framework — a set of lenses (Users vs. People, Entertain vs. Engage, Consumptive vs. Productive Friction) for judging whether a product idea, tool concept, or feature is genuinely meaningful to the humans it's for, or just performing usefulness while optimizing for engagement/attention. Use this whenever evaluating a NEW product/tool/feature concept before committing real effort to it ("should we build this", "is this idea worth pursuing", "what's the core insight here"), or when generating a new concept from scratch. Do NOT use this for routine code review, debugging, or technical implementation questions — it's an editorial/product judgment lens, not an engineering one. For reviewing written content or copy specifically, use neo-slow-media-editorial instead. For a narrow question about a single friction point in a flow, use neo-slow-media-productive-friction. For just the fast pre-ship gut-check, use neo-slow-media-final-question.
---

# Neo-Slow Media Editorial Lens

## What this is

A specific, opinionated point of view — not a generic "is this good UX"
checklist. It comes from one senior media editor and design researcher's
ongoing research and
practice (xiaojiahaina, "neo-slow media," 2021–present), and it exists to catch
a recurring failure mode: things that *look* useful or engaging but are
actually optimized to hold attention or check a box, rather than to change
something real for the person on the other end.

The full framework lives in `references/framework.md`, organized so you can
jump to just the section a given task needs rather than reading the whole
file every session: three lenses, a criteria checklist, four worked examples
(including one where the lenses disagree and one showing the framework
misapplied), five design movements for generative use, and four recurring
domain focus areas. Each item below points to the specific section it needs.
This skill is part of a small family — see "Related skills" at the bottom.

## When to apply this

**Product/tool/feature concepts** — before committing effort to building
something, or when asked to evaluate whether an idea is worth pursuing:
1. **Check the criteria checklist first** (`references/framework.md`). If the
   idea clearly fails it — an existing solution already works, it's a
   one-off task, it doesn't change a recurring behavior — say so and stop.
   Do not run the lenses looking for depth that isn't there: see the
   cautionary worked example in `references/framework.md` for exactly this
   failure mode (a 2-day fix turned into a 3-month build by running every
   lens reflexively instead of checking the checklist first).
2. If it's not an obvious fail, run the idea through the three lenses (Users
   vs. People / Entertain vs. Engage / Consumptive vs. Productive Friction).
   They don't always agree — see the worked example where Lens 2 and Lens 3
   conflict for what to do when they don't.
3. Ask the final editorial question: *"If someone engages with this well, every
   week, for a year — how are they different at the end of that year?"* This
   single question is usually the fastest way to separate a real idea from a
   plausible-sounding one.

**Generating a new idea, not just judging one** — when asked to brainstorm or
shape a concept from scratch rather than evaluate an existing one:
- Move through the five design movements in `references/framework.md`
  (listening → observation → experimentation → ideation → expression) instead
  of jumping straight to a pitch.
- If the concept sits in one of the four domain focus areas (future of work,
  future of learning, healing inventions, creative studio), name that domain
  explicitly — it sharpens what "too generic" existing solutions look like.

**When NOT to use this**: routine code review, debugging, architecture
decisions, or any purely technical implementation question. This is a judgment
lens for evaluating *what something is for and whether it's honest about it* —
not an engineering correctness tool. If a task is purely technical with no
product/content dimension, applying this lens will just add noise.

## How to share your read

The person you're talking to keeps the final call — you're offering a
sharper read, not handing down a ruling. Don't just recite the framework
back — apply it and share a genuine take, phrased so they can push back.
State:

1. Which lens (or lenses) is most relevant to this specific case, and why.
2. What the lens reveals that a surface read would miss (the "people problem
   under the user problem," the "entertains vs. engages" gap, which friction
   is consumptive vs. productive).
3. A direct answer to the final editorial question, and what that implies —
   worth the deeper investment, fine as a lightweight utility, or actually
   working against the person it claims to serve.
4. If the material is genuinely mixed (some good, some hollow) — say so
   specifically, per competency #6 (hold open the contradictions). Don't
   force a single take where the honest one is "this part is real, this
   part is performing usefulness."

Be direct and specific to the actual material in front of you — quote the
exact feature, phrase, or mechanic you're critiquing, the way an editor
marks up a specific line rather than commenting on a draft in the abstract.

## Related skills

- `neo-slow-media-editorial` — reviewing writing, copy, or messaging
  specifically (the seven editorial competencies).
- `neo-slow-media-productive-friction` — a narrow question about a single
  friction point in a flow, without the full product-worth-building
  evaluation.
- `neo-slow-media-final-question` — just the one-year question, for a fast
  pre-ship gut-check.
