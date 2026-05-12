# Memex State Architecture

> Memex State is a continuity runtime for reasoning across time.

Memex preserves structured continuity state so reasoning can continue across sessions, tools, files, and runtime boundaries.

Models perform reasoning compute.

Memex preserves the state structures that allow reasoning continuity to persist.

---

# Overview

Most AI systems treat each session as a mostly isolated interaction.

When the session ends, continuity often collapses into:

* partial summaries
* hidden assumptions
* scattered files
* lost execution context
* reconstructed memory
* fragile conversational history

Memex State is built around a different architectural model:

```text
continuity as explicit runtime state
```

The runtime is designed to preserve continuity through stable structures instead of relying on conversational reconstruction.

Memex organizes continuity around five architectural primitives:

```text
Compass = purpose
Snapshots = continuity time
Trails = memory
Loops = regulation
Reality = grounding
```

Together, these structures allow long-running AI-assisted work to remain inspectable, resumable, and grounded in observed reality.

---

# Architectural Boundary

Memex is not a reasoning engine.

Memex provides structured continuity state.

Models provide reasoning compute.

```text
Memex = continuity runtime
Model = reasoning compute
```

Memex is responsible for:

* continuity across time
* structured system state
* snapshot preservation
* trail preservation
* operational grounding
* resumable execution context
* continuity regulation

Models are responsible for:

* inference
* synthesis
* planning
* language reasoning
* interpretation

This boundary allows the reasoning engine to change while the continuity structure remains stable.

---

# Northstar Architecture

The public architecture of Memex is grounded in the Northstar model.

The Northstar defines the core continuity pattern:
The full Northstar continuity model is defined in [northstar.md](./northstar.md).

```text
Continuity = Regulate(Compass, Snapshots, Trails, Reality)
```

Memex does not attempt to preserve every token, message, or output.

It preserves the structured state required for reasoning continuity:

* purpose
* time
* memory
* grounding
* regulation
* lineage
* unresolved boundaries

The Northstar document is the conceptual spine of the public repository.

This architecture document describes how that spine is expressed as a runtime system.

---

# Compass

Compass defines persistent orientation.

A Memex system needs a stable way to evaluate whether continuity is drifting, improving, or losing direction.

Compass provides that orientation.

Without Compass:

* deviation has no meaning
* regulation has no reference point
* long-running work loses direction
* future state cannot be evaluated against purpose

In public terms, Compass represents the persistent purpose of the system.

It anchors continuity across changing sessions, tools, files, and models.

---

# Snapshots

Snapshots are the atomic unit of continuity.

A snapshot captures structured system state at a moment in time.

```text
snapshot₀ → snapshot₁ → snapshot₂ → snapshot₃
```

The newest snapshot represents the active continuity context.

Older snapshots move into memory through trails.

Snapshots may preserve:

* project state
* working state
* continuity lineage
* unresolved seams
* operational evidence
* continuity context

A snapshot is not merely a save file.

It is a structured continuity artifact.
Snapshot formation and continuity restoration are expanded in [snapshot-and-rehydration.md](./snapshot-and-rehydration.md).

---

# Trails

Trails preserve continuity behind the present moment.

Memex distinguishes between two major trail types.

## Main Trail

The Main Trail preserves structured continuity history.

It carries the system’s memory of past snapshots, decisions, seams, and state transitions.

## Operational Trail

The Operational Trail preserves observed reality.

Examples include:

* file changes
* command results
* runtime events
* artifact creation
* repository state changes
* execution evidence

Observed reality always outranks interpretation.

The Operational Trail exists so continuity can remain grounded in observable system behavior.
Operational continuity evidence is further described in [operational-trails.md](./operational-trails.md).

---

# Reality Grounding

Memex treats observed reality as a primary architectural constraint.

Continuity becomes fragile when generated summaries replace evidence.

Memex therefore attempts to preserve a separation between:

* observed runtime evidence
* declared state
* projected continuity views
* derived navigation layers

The runtime favors visible gaps over invented certainty.

If observed truth is missing, it should remain missing instead of being reconstructed from narrative context.

---

# Loops

Continuity is regulated through loops.

Loops compare continuity state against purpose, memory, and observed reality.

At a public architecture level, Memex uses two broad loop categories.

## Present Regulation

Present regulation keeps active continuity aligned with current observed conditions.

It compares:

* expected state
* observed state
* active continuity context
* operational evidence

This helps the system detect drift, instability, or unresolved state.

## Long-Horizon Improvement

Long-horizon processes operate across historical continuity.

They may support:

* reflection
* retrieval
* compression
* pattern analysis
* continuity improvement

These processes influence future continuity without rewriting observed history.

---

# Working State

Working state is the minimal active continuity nucleus.

It preserves the current execution boundary of the project.

Memex currently models working state through four core carriers:

* current objective
* current seam
* next action
* state summary

Working state is intentionally small.

Its purpose is not to explain everything.

Its purpose is to preserve enough structure for continuity to resume without manual reconstruction.

---

# Seams

A seam is an active unresolved boundary.

Seams represent the places where continuity, implementation, reasoning, or system behavior remains unsettled.

Examples include:

* architectural uncertainty
* runtime instability
* integration mismatch
* unresolved state transition
* validation failure
* routing uncertainty

A seam is not the same as a task.

The seam is the unresolved boundary.

The next action is the move applied to that boundary.

```text
current_seam != next_action
```

This distinction is part of continuity integrity.
The seam model is expanded in [seam-model.md](./seam-model.md).

---

# Rehydration

Rehydration restores active continuity state from stored snapshots.

Memex treats rehydration as continuity restoration, not memory approximation.

During rehydration, the system should not:

* invent missing state
* infer hidden context
* rewrite stored meaning
* collapse uncertainty into certainty
* replace source truth with narrative summary

Missing continuity remains visible.

The runtime prefers explicit gaps over fabricated continuity.

---

# Truth Semantics

Memex separates information into explicit truth classes.

This prevents observed reality, declared intent, projected continuity views, and derived navigation from collapsing into the same layer.

The public truth hierarchy is:
The complete public truth hierarchy is defined in [truth_semantics.md](./truth_semantics.md).

```text
Observed Truth
    ↓
Declared Truth
    ↓
Projected Truth
    ↓
Derived Truth
```

## Observed Truth

Observed truth is grounded in measurable runtime or workspace evidence.

Examples include file state, runtime events, operational trails, and execution ordering.

## Declared Truth

Declared truth is intentionally asserted state.

Examples include project purpose, current seam, next action, and continuity declarations.

## Projected Truth

Projected truth represents simplified continuity interaction surfaces.

Examples include working state, continuity summaries, and resume context.

## Derived Truth

Derived truth guides attention but does not define canonical state.

Examples include repo context maps, route cards, file classifications, and relevance rankings.

Derived navigation may help the system look in the right place.

Source truth still outranks it.

---

# Checkpoints

A checkpoint is a continuity snapshot.

It preserves validated continuity state at a point in time.

A checkpoint may contain:

* project metadata
* working state
* continuity lineage
* operational evidence
* continuity context

Checkpoints allow Memex to preserve continuity as structured runtime infrastructure rather than conversational memory.

---

# Continuity Lineage

Memex tracks continuity across time.

Lineage preserves:

* checkpoint ordering
* previous checkpoint references
* seam trajectory
* operational ordering
* workspace evolution

This allows a resumed session to recover not only what changed, but where the system existed within its continuity timeline.

---

# Repo Cognition

Memex includes a repository observation and navigation layer.

This layer exists to reduce structural fragmentation during long-running development work.

It may observe:

* workspace structure
* file classifications
* observed file changes
* repository organization
* route cards
* relevant implementation context

Repo cognition is derived navigation.

It guides attention.

It does not replace source truth.

Observed file contents remain authoritative.
Repository-derived continuity navigation is described further in [repo-cognition.md](./repo-cognition.md).

---

# Public Boundary

This public repository is intentionally curated.

It may contain:

* public architecture concepts
* sanitized examples
* research artifacts
* demos
* continuity models
* documentation surfaces

It does not contain:

* secrets
* credentials
* production continuity state
* private runtime internals
* private operational trails
* internal system prompts
* sensitive workspace artifacts

The public repository exposes architectural concepts while preserving operational boundaries.
The operational membrane behind the public continuity substrate is described in [public-boundary.md](./public-boundary.md).

---

# Current Status

```text
Experimental / Active Development
```

Memex State is currently focused on:

* continuity stabilization
* snapshot integrity
* rehydration reliability
* operational grounding
* truth semantics
* repo cognition
* public architecture convergence

The architecture is expected to evolve, but its core invariants remain stable:

* Compass anchors purpose
* Snapshots structure time
* Trails preserve memory
* Reality grounds observation
* Loops regulate continuity

---

# Closing Perspective

Memex does not attempt to simulate memory.

It treats continuity as infrastructure.

The goal is not to create the illusion of persistent intelligence.

The goal is to create systems where reasoning continuity can be:

* preserved
* inspected
* resumed
* validated
* grounded
* trusted

across long-running AI-assisted work.

At its smallest:

```text
Memex = continuity runtime
Model = reasoning compute
```

Memex preserves the conditions for reasoning continuity across time.
