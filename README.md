# tutoria-mentor

Strategic sparring partner skill for Claude Code.

## What It Does

`tutoria-mentor` is a Claude Code skill that acts as a strategic advisor through **compound memory** and **deliberate sparring**. Rather than executing tasks, it:

- Challenges assumptions and spots gaps in thinking
- References past decisions and patterns from accumulated context
- Generates novel options with clear tradeoffs
- Proposes concrete next steps

It improves with every conversation, building a knowledge base that gets smarter over time.

## Installation

Copy this directory to your Claude Code skills folder:

```bash
cp -r tutoria-mentor ~/.claude/skills/
```

Then invoke in Claude Code:

```
/tutoria-mentor [your strategic question]
```

## Understanding the Design

Read **[PHILOSOPHY.md](./PHILOSOPHY.md)** to understand why this skill is structured the way it is. Key properties to preserve:

- **Memory persistence** - compound knowledge across sessions
- **Sparring behavior** - challenge, don't validate
- **Open questions tracking** - nothing forgotten
- **Conversation-driven improvement** - grows from use, not maintenance
- **Frameworks as thinking tools** - not information dumps

## Core Files

| File | Purpose |
|------|---------|
| `SKILL.md` | Skill definition and protocols |
| `PHILOSOPHY.md` | Design principles and what to preserve |
| `context/` | Company context, team, priorities, blockers |
| `frameworks/` | Decision-making tools (AI leverage, team playbook, etc.) |
| `memory/` | Decisions made, learnings captured, session archives |
| `protocols/` | Self-improvement, sparring, delegation patterns |

## For Developers

Before auditing or evolving this skill, read `PHILOSOPHY.md` first. It captures what makes the skill valuable and what to preserve.

The self-improvement protocol (`protocols/self-improvement.md`) explains how the skill grows from conversations.
