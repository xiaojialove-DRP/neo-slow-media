# Neo-Slow Media — Agent Skills

A growing suite of ready-to-copy skills, built to the open
[Agent Skills specification](https://agentskills.io) (agentskills.io), that
apply xiaojiahaina's neo-slow media editorial framework. Four skills so far,
each with a narrow, specific trigger — pick the one (or ones) that match
what you're doing, rather than installing one skill that tries to cover
everything:

| Skill | Use it for |
|---|---|
| [`neo-slow-media-lens`](neo-slow-media-lens/) | The full evaluation: should we build this product/feature/tool? |
| [`neo-slow-media-editorial`](neo-slow-media-editorial/) | Reviewing writing, copy, or messaging specifically |
| [`neo-slow-media-productive-friction`](neo-slow-media-productive-friction/) | One narrow question: is this friction point worth keeping? |
| [`neo-slow-media-final-question`](neo-slow-media-final-question/) | A 5-second pre-ship gut-check, no full evaluation needed |

Because the suite follows the open spec rather than a vendor-specific
format, it's built to work anywhere that spec is implemented — that now
includes [Claude Code](https://claude.com/claude-code), Cursor, GitHub
Copilot / VS Code, OpenAI Codex, and Gemini CLI, among others. Installation
below is verified for Claude Code; other tools that support Agent Skills
should pick it up the same way, following their own docs for where skills
live.

See the [manifesto card](../README.md) or the full
[field guide](../FIELD-GUIDE.en.md) for the human-readable version of the
same framework.

## Install (Claude Code)

Copy whichever skills you want — you don't need all four:

```bash
cp -r neo-slow-media-lens ~/.claude/skills/
cp -r neo-slow-media-editorial ~/.claude/skills/
cp -r neo-slow-media-productive-friction ~/.claude/skills/
cp -r neo-slow-media-final-question ~/.claude/skills/
```

Claude Code picks up skills from `~/.claude/skills/` automatically.

## Install (other Agent Skills-compatible tools)

Check your tool's docs for where it expects skill folders — the skill
folders themselves don't need to change, only where you place them.

## The four skills

### `neo-slow-media-lens`

The flagship skill — the three lenses (Users vs. People, Entertain vs.
Engage, Consumptive vs. Productive Friction) applied together, plus the
criteria checklist and the final editorial question. Triggers when you ask
whether to build a new product, feature, or tool concept, or when
generating a new concept from scratch. The three lenses stay bundled here
because they check each other — see the worked example in
`references/framework.md` where Lens 2 and Lens 3 genuinely disagree.

**Input**: a feature idea or product concept, described in plain language.
**Output**: a stated position — which lens applies, what a surface read
would miss, and a direct answer to the final question. If the material is
genuinely mixed, it says so rather than forcing a single take.

> **You**: We want to add a "reading streak" badge to our news app — read an
> article every day, keep the streak alive. Worth building?
>
> **Agent**: This is Lens 2 territory — Entertain vs. Engage. A streak
> mechanic is the textbook entertain move: it produces a loss-aversion loop
> (don't break the streak) rather than a changed relationship to reading.
> Run the final question — if someone keeps this streak every day for a
> year, are they a better-informed person, or just someone with a longer
> streak? Most likely the second. If the goal is genuinely a reading habit,
> a productive-friction alternative — a weekly digest that asks "what's one
> thing from this week you'd explain to someone else" — does more for less
> mechanic.

### `neo-slow-media-editorial`

The seven editorial competencies, for reviewing writing, copy, or
messaging — a different audience and a different job than evaluating a
product concept, so it's a separate skill rather than a branch inside the
main one.

**Input**: a piece of copy, a paragraph, a messaging strategy.
**Output**: a marked-up read — quoting the exact phrase or mechanic, per
competency #6 ("hold open the contradictions") not forcing a tidy verdict
when the material is genuinely mixed.

### `neo-slow-media-productive-friction`

One narrow question, extracted from Lens 3 because it's the most
self-contained of the three — and the most frequent real-world moment
("should we remove this confirmation step") isn't the same moment as "should
we build this at all."

**Input**: a specific step, confirmation, delay, or constraint in a flow.
**Output**: whether that friction is consumptive (remove it) or productive
(keep or redesign around it) — with an explicit note that this alone
doesn't check whether the underlying goal is worth serving.

### `neo-slow-media-final-question`

Just the one-year question, for when a full evaluation is overkill and you
want one sharp check before you ship:

> "If someone engages with this well, every week, for one year — how are
> they different at the end of that year?"

## What's inside each skill

- `SKILL.md` — the trigger description and how-to-apply instructions the
  agent reads first.
- `neo-slow-media-lens/references/framework.md` — the full framework: three
  lenses, five design movements, domain focus areas, the criteria checklist,
  the final editorial question, and four worked examples (including one
  where the lenses disagree and one showing the framework misapplied). The
  other three skills are self-contained in their `SKILL.md` — no separate
  reference file needed for something this narrow.

This directory is a straight copy of the author's own working skills — not
simplified versions — so it stays in sync with how xiaojiahaina actually
applies the framework. The suite is expected to keep growing as the
practice does.
