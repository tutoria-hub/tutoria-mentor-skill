# Tutoria: Tech Stack

**Last updated:** 2024-12-04

---

## Architecture Overview

```
┌─────────────────────────────────────────────────────────────┐
│                     TUTORIA STACK                           │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  TUTORIA STUDIO              TUTORIA WEBAPP                 │
│  ───────────────             ─────────────                  │
│  Next.js 15 + React 19       Next.js (user-facing)          │
│  Cloudflare Workers          Cloudflare Workers             │
│  Cloudflare R2 (storage)     ElevenLabs (TTS)               │
│                              Mistral Voxtral (pronunciation)│
│                                                             │
│  Agentic curriculum          Parent/child interface         │
│  management + audio          + pronunciation checking       │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## Tutoria Studio

**Purpose:** Curriculum and audio management. Internal tool for content creation.

**Location:** `/Users/frederikhandberg/Tutoria-Stack/tutoria-studio/`

**Key features:**
- IPA-indexed sound system (maps phonemes to audio files)
- Content-addressed storage (SHA256 hash → automatic deduplication)
- Branch-based curriculum (parallel versions)
- Three-state validation (healthy/warning/broken)

**Agentic workflow:**
- Claude agents can: bulk create exercises, validate, check parity
- Humans must: generate audio (Eleven Labs GUI), crop waveforms, QA
- Sub-agent delegation saves 85-95% tokens on routine operations

**Key files:**
- `/CLAUDE.md` - Agent quick start
- `docs/ARCHITECTURE.md` - Deep technical dive
- `.claude/skills/tutoria-studio/SKILL.md` - Workflow protocols

---

## Tutoria WebApp

**Purpose:** User-facing application. What parents and children interact with.

**Location:** `/Users/frederikhandberg/Tutoria-Stack/tutoria-webapp/`

**Key features:**
- Pronunciation checking via Mistral Voxtral
- Audio playback from Studio CDN
- Progress tracking per child

**Pronunciation system:**
- Two-phase validation: blind hypothesis + contrastive scoring
- 75% threshold for pass (same for all phonemes - known issue)
- Edge cases: consonant clusters, short phonemes, hard sounds

**Known issues:**
- Consonant clusters (/bl/, /str/) fail inconsistently
- Per-phoneme difficulty not accounted for
- Spec created: `docs/specs/pronunciation-edge-case-investigation.md`

---

## External Services

| Service | Purpose | Notes |
|---------|---------|-------|
| Cloudflare Workers | Serverless compute | Both Studio and WebApp |
| Cloudflare R2 | Object storage | Audio files, curriculum JSON |
| ElevenLabs | Text-to-speech | Audio generation in Studio |
| Mistral Voxtral | Audio analysis | Pronunciation validation |

---

## Development Approach

**AI-native development:**
- Frederik uses Claude Code for all development
- Tutoria Studio has skill for agentic workflows
- Ash learning AI-native patterns (4-week training plan exists)

**Key principle:** AI handles execution, humans keep taste and direction.
