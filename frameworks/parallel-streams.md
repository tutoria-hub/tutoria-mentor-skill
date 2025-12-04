# Tutoria Parallel Streams

The core workstreams that must run simultaneously.

**Last updated:** 2024-12-04

---

## The Four Streams

```
┌─────────────────────────────────────────────────────────────────┐
│                    TUTORIA PARALLEL STREAMS                     │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  1. PRODUCT ENGINE                                              │
│     Studio (curriculum/audio) + WebApp (UX)                     │
│     Owner: Frederik + Ash                                       │
│     Goal: Solid, bug-free, pronunciation works                  │
│                                                                 │
│  2. UK PARENT ACQUISITION                                       │
│     Content marketing, SEO, parent communities                  │
│     Owner: Julie + Jakub (with AI scale)                        │
│     Goal: First 10 paying UK parents                            │
│                                                                 │
│  3. VALIDATION (Denmark)                                        │
│     Test schools, feedback collection                           │
│     Owner: Julie + Jakub (in person)                            │
│     Goal: Prove it works, get testimonials                      │
│                                                                 │
│  4. LEARNING LOOP                                               │
│     Track outcomes, not just usage                              │
│     Owner: Frederik (system) + Lone (interpretation)            │
│     Goal: Prove kids actually improve                           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Stream Dependencies

```
PRODUCT must be stable → before UK ACQUISITION scales
VALIDATION provides proof → feeds UK ACQUISITION messaging
LEARNING LOOP proves outcomes → enables both VALIDATION and ACQUISITION
```

**Current bottleneck:** Product stability. Can't scale acquisition until pronunciation works consistently.

---

## Stream 1: Product Engine

**What's in scope:**
- Bug fixes (WebApp UX issues)
- Pronunciation edge cases
- Curriculum completion (last 5%)
- Parent dashboard improvements

**What's out of scope:**
- New major features
- B2B-specific features
- Mobile app

**Current priority:** Pronunciation investigation → fix edge cases → curriculum polish

---

## Stream 2: UK Parent Acquisition

**Channels identified:**
- Facebook dyslexia parent groups
- British Dyslexia Association (potential partnership)
- Mumsnet/Netmums SEN sections
- Homeschool communities (Ambleside Online)
- Regional dyslexia associations

**First 10 customer plan:**
1. Join groups, be helpful (build presence)
2. DM struggling parents, offer free access for feedback
3. Collect testimonials
4. Post about Tutoria with permission
5. Then run paid ads with social proof

**Jakub's role:** Authentic dyslexia story is key marketing asset

---

## Stream 3: Validation (Denmark)

**Purpose:**
- Keep test schools engaged
- Collect specific feedback
- Get testimonials for UK marketing
- Understand what breaks in real usage

**Activities:**
- School visits
- Feedback collection (structured)
- Relationship maintenance

**Output:** Testimonials, bug reports, usage insights

---

## Stream 4: Learning Loop

**Current state:** Progress through stages only

**Target state:** Visible learning outcomes parents can see and share

**Options being considered:**
1. Pre/post diagnostic per stage
2. Word recognition count ("Week 1: 2 words → Week 4: 8 words")
3. Parent-reported improvements

**Why it matters:**
- Parents buy hope, not software
- "My child improved" is the marketing message
- Proof enables word-of-mouth

---

## Resource Allocation

| Person | Stream 1 | Stream 2 | Stream 3 | Stream 4 |
|--------|----------|----------|----------|----------|
| Frederik | Primary | - | - | Build system |
| Ash | Primary | - | - | - |
| Julie | - | Secondary | Primary | - |
| Jakub | - | Primary | Secondary | - |
| Lone | - | - | - | Interpret |

**Note:** Julie + Jakub split between streams 2 and 3. May need to specialize later.

---

## Stream Health Check

Ask weekly:

1. **Product:** Is pronunciation working? How many bugs reported?
2. **UK Acquisition:** How many parents contacted? Any conversions?
3. **Validation:** Any school feedback this week? Testimonials collected?
4. **Learning Loop:** Can we show progress? What data do we have?
