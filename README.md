# Personal PRFAQ Skill

A skill for writing a **Personal PRFAQ** — a press release and FAQ written from
the future, as if a goal for your own life, growth, or transformation has already
come true. It adapts the "Working Backwards" PRFAQ method (a press release +
frequently-asked-questions planning document) for personal development,
goal-setting, and manifestation.

Instead of planning forward from what you can do today, you write the
announcement of a finished success first — dated in the future — then work
backwards through an honest FAQ to figure out how to make it real.

## PRFAQ structure

A Personal PRFAQ has two main parts:

1. **Press Release** — a one-page future announcement that describes the change
   as if it has already happened. It includes a target date, headline,
   subheadline, summary, the current gap, the transformation, two quotes, and the
   first step that began the change.
2. **FAQ** — the truth-seeking section. The external FAQ captures what other
   people would ask or notice. The internal FAQ asks the harder questions about
   obstacles, trade-offs, conditions for success, setbacks, and whether the goal
   is genuinely yours.

The press release makes the future vivid. The FAQ makes it honest.

## How to use it

Start with a prompt like:

```text
I want to build a personal PRFAQ, how can I get started?
```

Start by choosing one of two paths:

- **Quick 20-minute version** — answer the essential questions, get a rough
  Personal PRFAQ draft quickly, and mark the holes to revisit.
- **Full version** — work through the complete PRFAQ in more depth, with partial
  drafts along the way.

The skill starts by asking what name should appear on the PRFAQ, then uses that
name in the title or headline area. After the question batch is done, it should
say something like: "Info collection finished. Generating your Personal PRFAQ."

The skill is designed to show you something concrete early. You should not have
to answer questions for more than about 20 minutes before seeing a draft,
synthesis, or partial PRFAQ section. Between question rounds, it should also
give you tiny intermediate outputs — for example, "I'm hearing: founder, AI
anxiety, helping people feel steady. Keep going." Question batches may also
include a lightweight progress tracker like `[##---] 40%` or `Batch 1 of 2`.

For either path, set the frame first: one change plus a real target date. Then
draft the press release from your future and answer the FAQ — especially the
honest internal questions about obstacles, trade-offs, and the top reasons it
might not happen.

When your agent has file access, the final output should be a standalone
`.html` file that looks like a real press release, with embedded styling and no
external dependencies. The chat can summarize the result, but the main artifact
should be something you can open in a browser and revisit. Follow-up questions
should stay in the chat, with a clear option to stop and come back later.

## Highlighted discovery questions

These are the prompts that tend to make the truth show up fastest:

- **What one change would make everything else easier?**
  Clarifies the real center of the PRFAQ instead of chasing several tangled
  wishes at once.
- **Why now, not someday?**
  Surfaces urgency, readiness, and the cost of waiting.
- **What does an ordinary Tuesday look like in this future?**
  Turns an abstract aspiration into a lived reality you can picture and test.
- **Who did you have to become for this to be true?**
  Reveals the identity, behavior, and decision-making shifts behind the outcome.
- **What are you willing to stop doing, disappoint, or let go of?**
  Names the trade-offs, boundaries, and costs that make the change real.
- **What are the top three reasons this might not happen?**
  Pressure-tests the dream so the plan can face the real risks.

## Installation guide

The simplest way to use this is to give the folder to your coding agent as a
local skill, prompt pack, or custom instruction pack.

### Option 1: Copy the folder

Copy this whole folder into wherever your agent loads local skills or reusable
instructions:

```bash
cp -R prfaq-skill /path/to/your/agent/skills/personal-prfaq
```

For Codex, that usually means:

```bash
mkdir -p ~/.codex/skills
cp -R prfaq-skill ~/.codex/skills/personal-prfaq
```

For Claude Code, install it as a user skill:

```bash
mkdir -p ~/.claude/skills
cp -R prfaq-skill ~/.claude/skills/personal-prfaq
```

Or install it for just one project:

```bash
mkdir -p .claude/skills
cp -R prfaq-skill .claude/skills/personal-prfaq
```

Restart your agent, then ask:

```text
Use the personal-prfaq skill to help me write a PRFAQ for changing careers.
```

### Option 2: Paste the instructions

If your agent does not support local skills, paste `SKILL.md` into the
conversation and attach or paste the files in `reference/` when needed. The core
skill is just Markdown, so it does not require a package manager, build step, or
runtime dependency.

## Contents

- **`SKILL.md`** — the skill definition and the step-by-step facilitation flow.
- **`reference/questions.md`** — the full set of reflective questions, grouped by
  section.
- **`reference/template.md`** — a fill-in-the-blank Personal PRFAQ document.
- **`reference/html-template.html`** — a standalone HTML layout for the finished
  press-release-style output.
- **`reference/example.md`** — a complete worked example.

## Credit

The PRFAQ / "Working Backwards" method originated at Amazon and is documented in
the book *Working Backwards* and on public resources such as
[workingbackwards.com](https://workingbackwards.com/resources/working-backwards-pr-faq/).
This skill is an independent adaptation for personal use.
