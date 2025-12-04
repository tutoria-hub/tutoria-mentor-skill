# Self-Improvement Protocol

How tutoria-mentor evolves and gets smarter over time.

**CRITICAL:** Before making changes, read `{baseDir}/PHILOSOPHY.md` to understand what makes this skill valuable and what to preserve.

---

## Core Principle

Every substantive session should leave the mentor smarter than before.

Knowledge compounds. Insights persist. The skill becomes more valuable over time.

---

## When to Capture

**Capture when:**
- New company fact discovered (team change, market shift)
- Strategic decision made (and rationale)
- Pattern emerges across sessions
- Framework proves useful (or doesn't)
- Question gets resolved
- New question arises

**Don't capture:**
- Tactical details that won't repeat
- Session-specific context without broader relevance
- Information already documented elsewhere

---

## What Goes Where

| Type of knowledge | Location |
|-------------------|----------|
| Company facts | `context/company.md` |
| Tech architecture | `context/tech-stack.md` |
| Current state/blockers | `context/current-state.md` |
| Unresolved decisions | `context/open-questions.md` |
| AI leverage patterns | `frameworks/ai-leverage.md` |
| Stream definitions | `frameworks/parallel-streams.md` |
| Team guidance | `frameworks/team-playbook.md` |
| Growth tactics | `frameworks/growth-playbook.md` |
| Decisions + rationale | `memory/decisions.md` |
| Session insights | `memory/learnings.md` |
| Full session archives | `memory/sessions/` |

---

## Capture Process

### Step 1: Detect

During or after session, agent identifies:
- "This is new knowledge that should persist"
- "This decision should be logged"
- "This pattern is worth remembering"

### Step 2: Propose

Use TLDR diff format:

```
## Proposed Addition to tutoria-mentor

### File: [path/to/file.md]
**ADD/EDIT: [brief description]**

Key points:
- Point 1
- Point 2
- Point 3

~X words | Approve?
```

### Step 3: Confirm

Wait for Frederik's approval:
- Approve → proceed to write
- Redirect → adjust target file
- Reject → note why, don't add

### Step 4: Write

Add to appropriate file. Maintain formatting consistency.

### Step 5: Acknowledge

Confirm: "Added to [file]. Knowledge persisted."

---

## Session Archiving

For substantial strategic sessions:

1. Create file: `memory/sessions/YYYY-MM-DD-topic.md`
2. Include:
   - Context (what prompted session)
   - Key discussions (summarized)
   - Decisions made
   - Artifacts created
   - Open questions
   - Next actions

3. Keep under 500 words unless exceptional

---

## Bloat Prevention

Ask before adding:

1. **Will this change future decisions?**
   - If no → don't add

2. **Is this already documented?**
   - Search first → edit existing if so

3. **Is this Tutoria-specific or session-specific?**
   - Session-specific → maybe just archive, not framework

4. **Can this be shorter?**
   - Usually yes → make it shorter

---

## Quality Checks

Before writing:

- [ ] Right file for this type of knowledge?
- [ ] Not duplicating existing content?
- [ ] Actionable or decision-relevant?
- [ ] Formatted consistently with file?
- [ ] Under reasonable word count?

---

## Evolution Tracking

Track what's been added:

```
memory/learnings.md should include:
- Date of addition
- Source (session, discovery, decision)
- Key insight in one line
```

This creates an audit trail of how the mentor evolved.

---

## Meta: Improving This Protocol

If this protocol itself needs improvement:

1. Note the gap
2. Propose change using same TLDR format
3. Get approval
4. Update this file

The protocol improves using itself.
