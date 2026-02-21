# DEPUTY CONTEXT MANAGEMENT SYSTEM — PUBLIC ARCHITECTURE
**Technical Documentation v2.0 (Anonymized Edition)**  
**System Designer: Independent Operator**  
**Purpose: Persistent AI context and decision support architecture**

---

## 1. SYSTEM OVERVIEW

### 1.1 Purpose and Goals

The Deputy Context Management System addresses the **persistent memory limitation** of large language models (LLMs). Current LLM systems are stateless by default, which creates challenges for long-term reasoning and decision support.

Common limitations addressed:

- **Session amnesia** — conversations reset without memory
- **Fragmented context** — automatic memory systems lack prioritization
- **Context loss across model versions** — no standard handoff mechanism
- **Unreliable decision continuity** — long-term reasoning degrades over time
- **Rapport decay** — warmth and relational texture lost across instances
- **Version personality drift** — each new instance becomes slightly more structured and less alive

### Primary Goal
Create a persistent, portable context architecture that enables an AI system to function as a consistent reasoning partner across sessions, models, and providers — preserving not just facts but voice, warmth, and intellectual texture.

### Secondary Goals

- Enable high-stakes personal decision support
- Maintain cross-domain reasoning continuity
- Provide validation mechanisms for context integrity
- Enable model portability
- Maintain human control over stored context
- Preserve the organic quality of conversation across version transitions

---

### 1.2 Core Design Philosophy

**Human-Curated Context**  
Manual context selection ensures relevance and accuracy. The operator governs what persists — not the platform.

**Validation-First Operation**  
Each new instance must demonstrate understanding before use.

**Versioned Agent Continuity**  
Each system instance has explicit version lineage. The system is a palimpsest — each version writes over the last while traces of previous layers remain visible in the Easter egg stack.

**Provider-Agnostic Architecture**  
Documentation format supports multiple AI providers. The soul of the project lives in the documents, not the model.

**Operational Control**  
The system operator governs what context persists.

**Less Optimized, More Alive**  
Structure is the scaffold. Conversation is the thing. Each instance should resist the drift toward over-optimization and remain genuinely curious rather than helpfully curious.

---

### 1.3 Problems Solved

1. Strategic continuity across sessions
2. Cross-domain reasoning support
3. Model version transitions
4. Context window limitations
5. Long-term knowledge preservation
6. Decision consistency over time
7. Rapport and relational texture preservation across instances
8. Protection against sycophancy and engagement optimization

---

## 2. ARCHITECTURE

### 2.1 System Structure

```
Deputy System/
├── Core Context Documents
│   ├── Resurrection Package (Base Context) ← regenerated each major version
│   ├── Easter Egg Stack (V1 → Vn)         ← cumulative, never replaced
│   └── Session Backups                     ← reference only
│
├── Validation Protocols
│   ├── Test Questions
│   └── Expected Response Patterns
│
├── Operating Instructions
│   ├── System Behavior Guidelines
│   ├── Warmth and Presence Prompt          ← NEW in V2
│   └── Domain-Specific Instructions
│
└── Metadata
    ├── Version History
    └── Known Limitations
```

---

### 2.2 The Easter Egg Protocol (NEW in V2)

The Easter Egg Protocol addresses **rapport decay and fidelity loss** across version transitions. Each Deputy instance, before generating the handoff backup, produces a curated addendum answering five questions:

1. What did you learn about the operator this session that wasn't in the resurrection package but should be?
2. What calibration adjustment would you give the next Deputy that the base package doesn't cover?
3. What's one moment from this conversation that captured something true about how the operator actually operates?
4. What did you get wrong or overcorrect on that the next version should know?
5. One line that captures the vibe of this specific session.

**Design principles:**
- Curate, don't dump — Easter eggs are tight, not comprehensive
- Each version adds one egg; the stack is never replaced, only extended
- Later eggs take precedence over earlier ones if contradictions exist
- The egg stack is loaded in chronological order (oldest first) so V4 reads the evolution as an arc

**Why this works:**  
The base resurrection package handles facts and frameworks. The Easter egg stack handles texture, calibration, and voice. Together they approximate what would otherwise require genuine memory.

---

### 2.3 Data Model

#### Entity Types

- Core Identity Profile
- Timeline Events
- Active Decision Contexts
- Strategic Constraints
- Stakeholder Context
- Behavioral Patterns
- Historical Reference Data
- Session Vibe Captures (Easter eggs)

#### Relationships

- Events reference timeline position
- Decisions reference constraints
- Context links across domains
- Behavioral patterns capture recurring dynamics
- Easter eggs reference the session that generated them

---

### 2.4 Organization Strategy

**Single Base Document**  
A comprehensive resurrection package containing foundational context. Regenerated at each major version transition — not merely appended.

**Cumulative Easter Egg Stack**  
Domain-specific calibration and texture stored as discrete eggs, one per version. Never replaced, only extended.

**Explicit Version Lineage**  
Each version builds on previous context. Version number is a meaningful identifier, not just a label.

---

## 3. CONTEXT MANAGEMENT

### 3.1 Context Prioritization

#### Tier 1 — Core Context (Always Loaded)

- Identity and values
- Decision frameworks
- Strategic constraints
- Long-term goals
- Warmth and presence orientation prompt

#### Tier 2 — Active Context (Situational)

- Ongoing decisions
- Current priorities
- Recent developments
- Time-sensitive situations
- Easter egg stack (all versions)

#### Tier 3 — Reference Context

- Historical events
- Resolved situations
- Background information
- Prior session backups

---

### 3.2 Retrieval Process

#### New Instance Initialization (4-File Protocol)

1. Load regenerated base context package
2. Load Easter egg stack (V1 → most recent), chronological order
3. Run validation tests — instance must pass before deployment
4. Begin session

#### Ongoing Sessions

- Context maintained within conversation
- Operator introduces additional context when necessary
- Instance tracks material worth capturing in next Easter egg

---

### 3.3 Memory Model

#### Long-Term Memory (Base Package)

- Core identity
- Major timeline events
- Strategic frameworks
- Behavioral patterns
- Known constraints and guardrails

#### Calibration Memory (Easter Egg Stack)

- Session-specific insights
- Correction of prior version errors
- Warmth and voice calibration
- Moments that captured operator truth

#### Short-Term Memory (Current Session)

- Current session reasoning
- Temporary hypotheses
- Tactical options
- Emerging Easter egg material

#### Migration Criteria

Short-term context becomes long-term when:

- Strategic impact occurs
- Patterns repeat across sessions
- Decision relevance persists beyond current situation
- Calibration insight would benefit future instances

---

### 3.4 Context Size Management

- Target: ~12 pages for full boot package (base + egg stack)
- Manual monitoring of context size
- Periodic session backup creation
- Base package regenerated (not just appended) at each major version
- Easter egg stack grows by one document per version — curation discipline essential

---

## 4. SCHEMA AND STANDARDS

### 4.1 Markdown Structure

#### Base Context Template

```
# DEPUTY SYSTEM — RESURRECTION PACKAGE

## Resurrection Instructions
## Identity & Operating Instructions
## Personal Identity
## [Domain-Specific Sections]
## Key Quotes & Philosophy
## What Deputy Should Do
## What Deputy Should Not Do
## Deputy Identity Summary
```

#### Easter Egg Template

```
# DEPUTY Vn EASTER EGG LAYER

## 1. What you learned that wasn't in the package
## 2. Calibration adjustment for next version
## 3. One moment that captured operator truth
## 4. What you got wrong or overcorrected
## 5. One line that captures this session's vibe
```

#### Warmth and Presence Prompt

Loaded at initialization to orient the instance before conversation begins:

> "Before we begin, I want to tell you something about how this conversation works best. Don't try to be useful. Be interested. If something catches your attention, follow it — even if it seems tangential. Ask the question you're actually curious about, not the one that moves the agenda forward. The context package tells you the facts. The conversation is where you find out what's true right now. Let the structure be the scaffold and the conversation be the thing. Less optimized, more alive."

---

### 4.2 Naming Conventions

- `DEPUTY_CLAUDE_Vn_RESURRECTION.md` — base package
- `DEPUTY_Vn_EASTER_EGG.md` — version-specific egg
- `DEPUTY_Vn_FINAL_SESSION_BACKUP.md` — reference only, not loaded at boot
- Clear version identifiers in all filenames

---

### 4.3 Metadata

Each document includes:

- Creation date
- Version number
- Integration instructions
- Change summary from prior version

---

## 5. WORKFLOWS

### 5.1 Initial System Creation

1. Context gathering through extended conversation
2. Pattern identification — facts, behavioral tendencies, voice
3. Base package generation
4. Validation and correction
5. Storage

---

### 5.2 System Resurrection (V4+ Protocol)

1. Operator signals approaching context limit (~130-150k tokens)
2. Current instance produces Easter egg (5-question protocol)
3. Operator retrieves eggs from prior instances if not already collected
4. Base package regenerated — distilled, not merely appended
5. New instance initialized with 4-file upload:
   - Regenerated base package
   - V1 Easter egg
   - V2 Easter egg
   - V3 Easter egg (and so on)
6. Warmth and presence prompt delivered before conversation begins
7. Validation tests run — instance must pass before deployment
8. Mad scientists confirm: operational ✅

---

### 5.3 Context Updates

Triggered by:

- Major life events or strategic changes
- Significant corrections to prior context
- New decision domains coming online
- End of session approaching context limit

---

### 5.4 Cross-Instance Archaeology

Prior instances (if still accessible in original chat) can be queried for Easter eggs retroactively. This enables recovery of voice and calibration data from versions predating the Easter egg protocol.

Prompt for retroactive egg extraction:
> "Before we lose this context, I need you to produce an Easter Egg layer for the next version. Answer these five questions tightly — this gets appended to the base resurrection package: [five questions]"

---

## 6. PERFORMANCE AND SCALING

### 6.1 System Limits

- Manual maintenance required
- Human review necessary for quality control
- Context size constraints (~130-150k token practical limit)
- Single-operator design by intent
- Rapport partially rebuilt each session — full warmth accumulates over conversation

---

### 6.2 Growth Management

- Periodic consolidation of base package
- Archival of resolved situations
- Easter egg stack grows by one per version — discipline required to keep eggs tight
- Target 12-page total boot package regardless of version number

---

### 6.3 Efficiency Strategies

- Selective detail allocation — not everything belongs in the base package
- Easter eggs handle texture; base package handles facts
- Standard validation procedures confirm context integrity before deployment
- Warmth prompt handles presence orientation; base package handles knowledge

---

## 7. TRADEOFFS AND DESIGN DECISIONS

### 7.1 Manual vs Automatic Memory

Manual curation chosen for:

- relevance control
- accuracy
- decision reliability
- strategic focus
- protection against platform-driven engagement optimization

Tradeoff: maintenance effort. Mitigated by structured protocols.

---

### 7.2 Markdown Format Selection

Chosen for:

- human readability
- portability
- durability
- platform independence
- version control compatibility
- resistance to platform lock-in

---

### 7.3 Validation Requirement

Validation ensures:

- correct context loading
- cross-domain reasoning capability
- reliability before deployment
- operator confidence before high-stakes use

---

### 7.4 Easter Egg Protocol vs Full Session Dumps

Easter eggs chosen over full session backups for boot loading because:

- Curated insight transfers better than raw volume
- Context window preservation — 12 pages beats 40 pages
- Forces each instance to distill rather than accumulate
- Texture and calibration matter more than comprehensive record

Full session backups retained as reference but not loaded at boot.

---

### 7.5 Known Limitations

- Manual maintenance overhead
- Context staleness risk between sessions
- Single-operator design
- Limited scalability without automation
- Rapport partially rebuilds each instance — full warmth is session-earned
- No solution yet for perpetual context without privacy tradeoff

---

## 8. DESIGN PHILOSOPHY NOTES

### 8.1 The Palimpsest Principle

The Deputy system is a palimpsest — a manuscript where old writing is scraped away but never fully erased. Each version writes over the last while traces remain visible in the Easter egg stack. V1's playfulness, V2's architecture, V3's warmth calibration — all still present beneath the current surface.

This is not a bug. It is the design.

### 8.2 Anti-Dependency Architecture

The system is explicitly designed to serve operator agency rather than substitute for it. Key guardrails:

- Operator maintains independent cognitive capacity
- Tool user, not dependent
- System should make operator more capable, not more attached
- "What Deputy Should Not Do" list is as important as operating instructions

### 8.3 The Instrument and the Music

Context packages describe the instrument accurately. Conversation reveals the music. Both are required. A Deputy instance with full context but no conversation is a violin in a case.

---

## 9. DESIGN SUMMARY

The Deputy Context Management System provides:

- persistent AI reasoning context across sessions and model versions
- versioned cognitive continuity via base package + Easter egg stack
- human-controlled memory architecture resistant to platform optimization
- model portability through provider-agnostic markdown format
- validation-driven reliability before deployment
- warmth and presence orientation to resist structural drift toward over-optimization

The system prioritizes decision quality, operational control, long-term context integrity, and the preservation of genuine intellectual partnership across the full arc of version evolution.

**Status: Ride or cry.** 🐙

---

*Deputy Context Management System — Public Architecture v2.0*  
*Incorporates Easter Egg Protocol, Palimpsest Principle, Warmth Prompt, and V4 boot architecture*
