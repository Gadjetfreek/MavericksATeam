# ADR-0007 — Elevate Principles into the Platform

**Status:** Accepted
**Date:** 2026-07-30
**Decision Owner:** Architecture Council (Chat, Jeebs, User)

---

# Background

During development of the HomeBuyer Experts platform, we identified a recurring pattern:

Significant architectural decisions were being rediscovered through conversation rather than inherited through the platform.

The discussion surrounding project constitutions, governance, AI context recovery, and documentation revealed that many "project decisions" were actually **platform decisions** that should benefit every future project.

This ADR establishes a formal process for recognizing and promoting those discoveries into MavericksATeam itself.

---

# Decision

MavericksATeam shall become a **learning platform**, not merely a project repository.

When a principle proves valuable beyond a single project, it will be elevated into the platform so that future projects inherit it automatically.

Projects should improve MavericksATeam.

MavericksATeam should improve every future project.

---

# Platform Hierarchy

Every project will follow this hierarchy.

```
MavericksATeam
│
├── CONSTITUTION.md
├── GOVERNANCE.md
├── AGENTS.md
├── templates/
│
└── projects/
    └── <project>/
        ├── CONSTITUTION.md
        ├── PROJECT-BRIEF.md
        ├── CURRENT-STATE.md
        ├── HANDOFF.md
        ├── NEXT-STEPS.md
        └── DECISIONS.md
```

---

# Institutional Changes

## 1. Project Constitutions

Every project shall contain its own `CONSTITUTION.md`.

Purpose:

Define **why the project exists** and identify its First Principle.

Examples:

* HomeBuyer Experts → "What is best for the buyer?"
* Healthcare → "What is best for the patient?"
* Education → "What is best for the learner."

Project constitutions inherit the MavericksATeam Constitution but define mission-specific philosophy.

---

## 2. Separate Philosophy from Operations

Documentation responsibilities shall remain distinct.

| Document | Responsibility |
| ------------- | --------------------- |
| CONSTITUTION | Enduring philosophy |
| GOVERNANCE | Decision authority |
| ARCHITECTURE | Technical design |
| PROJECT-BRIEF | Mission |
| CURRENT-STATE | Current progress |
| HANDOFF | Session continuity |
| DECISIONS | Architectural history |

No document should attempt to perform multiple roles.

---

## 3. Repository as Institutional Memory

Conversations are temporary.

Documentation is permanent.

Whenever an architectural decision is reached, it should be documented during the same work session.

Future contributors should inherit decisions—not reconstruct them.

---

## 4. AI Startup Sequence

Before strategic work begins, AI agents should load context in the following order:

1. MavericksATeam Constitution
2. Governance
3. Agent Charter
4. Project Constitution
5. Project Brief
6. Current State

This establishes philosophy before implementation.

---

## 5. Promote Repeated Decisions

Whenever the same architectural question is answered more than once, ask:

> "Should this become part of MavericksATeam?"

If the answer is yes, create or update the appropriate platform documentation, template, or governance artifact.

Repeated decisions indicate missing platform capability.

---

## 6. Optimize for the Next Contributor

Every significant change should reduce the effort required for the next human or AI contributor to understand the project.

Institutional knowledge belongs in documentation—not individual memory.

---

## 7. Project Readiness Requirement

Implementation should not begin until the following exist:

* Project Constitution
* Project Brief
* Current State
* Initial Decision Log

Projects without these artifacts are considered incomplete foundations.

---

# Implementation Tasks

The following work should be completed within MavericksATeam.

### Platform

* [x] Create root `CONSTITUTION.md`.
* [ ] Review `GOVERNANCE.md` for alignment with the Constitution.
* [x] Update `AGENTS.md` to require loading the Constitution before project work.
* [x] Add ADR templates.

### Templates

Create reusable templates for:

* [x] `CONSTITUTION.md`
* [x] `PROJECT-BRIEF.md`
* [x] `CURRENT-STATE.md`
* [x] `HANDOFF.md`
* [x] `NEXT-STEPS.md`
* [x] `DECISIONS.md`

These become the default starting point for every future project.

### AI Workflow

Update all AI agent charters to:

* [x] Load philosophy before implementation.
* [x] Promote reusable discoveries into MavericksATeam.
* [x] Record architectural decisions as ADRs.
* [x] Prefer documentation over long conversational context.

---

# Expected Outcome

MavericksATeam evolves from a collection of repositories into a continuously improving operating system.

Every completed project strengthens the platform.

Every new project begins with more wisdom than the one before it.

The platform becomes increasingly resilient, consistent, and maintainable as knowledge compounds over time.

---

# Guiding Principle

> **Whenever we discover a principle that applies beyond the current project, we stop treating it as a project decision and elevate it into MavericksATeam.**

This is how the platform learns.
