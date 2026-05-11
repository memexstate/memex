# Truth Semantics

> Continuity systems become unstable when observation, interpretation, projection, and navigation collapse into the same layer.

Memex State separates continuity information into explicit truth categories.

This helps the runtime:

* preserve continuity clarity
* reduce semantic drift
* distinguish evidence from interpretation
* expose uncertainty instead of hiding it
* maintain stable resumability across time

Truth semantics are treated as part of continuity infrastructure.

---

# Why Truth Semantics Exist

Long-running AI systems accumulate information from many sources.

Examples include:

* runtime observations
* filesystem state
* generated summaries
* continuity declarations
* operational evidence
* inferred interpretations
* navigation structures

Without semantic separation, these layers gradually blur together.

As this drift compounds:

* assumptions become difficult to distinguish from evidence
* summaries replace operational grounding
* projected structures appear authoritative
* continuity reconstruction becomes unstable

Memex attempts to reduce this collapse through explicit truth semantics.

---

# The Core Truth Classes

Memex currently models four primary truth classes.

```text
Observed Truth
    ↓
Declared Truth
    ↓
Projected Truth
    ↓
Derived Truth
```

Each class serves a different role within continuity.

---

# Observed Truth

Observed truth is grounded in measurable operational evidence.

Examples may include:

* filesystem state
* runtime events
* execution ordering
* operational trails
* workspace changes
* repository state

Observed truth exists to keep continuity grounded in observable reality.

Observed operational evidence remains authoritative.

---

## Design Characteristics

Observed truth should:

* remain evidence-backed
* remain inspectable
* avoid reconstruction from summaries
* preserve operational grounding

The runtime intentionally prefers missing observed truth over fabricated observed truth.

---

# Declared Truth

Declared truth is intentionally asserted continuity state.

Examples may include:

* project purpose
* current seam
* next action
* continuity summaries
* architectural decisions
* milestone declarations

Declared truth preserves intentionally stated continuity context.

---

## Design Characteristics

Declared truth should:

* remain explicit
* preserve semantic intent
* avoid silent mutation
* remain distinguishable from observed evidence

The runtime may normalize structure.

It should avoid rewriting meaning.

---

# Projected Truth

Projected truth represents continuity-oriented execution surfaces derived from continuity state.

Examples may include:

* working state
* continuity views
* resume context
* continuity summaries

Projected truth exists to simplify continuity interaction surfaces without replacing underlying continuity state.

---

## Design Characteristics

Projected truth should:

* remain structurally stable
* preserve continuity shape
* reduce semantic drift
* remain connected to continuity context

Projected continuity surfaces should avoid inventing missing state.

---

# Derived Truth

Derived truth consists of navigation and continuity-guidance structures.

Examples may include:

* route cards
* repo context maps
* file classifications
* structural groupings
* relevance ranking
* contextual navigation surfaces

Derived systems guide attention.

They do not define canonical continuity authority.

---

## Design Characteristics

Derived truth may:

* reduce navigation fragmentation
* compress structural complexity
* preserve contextual navigation
* surface relevant continuity context

But:

```text
source truth remains authoritative
```

Observed reality outranks derived navigation.

---

# Semantic Stability

Truth semantics only remain useful if core meanings remain stable.

Memex attempts to preserve semantic consistency for continuity-critical concepts.

Examples include:

| Term              | Meaning                                         |
| ----------------- | ----------------------------------------------- |
| Current Seam      | Active unresolved boundary                      |
| Next Action       | Immediate move applied to seam                  |
| Snapshot          | Structured continuity state at a moment in time |
| Rehydration       | Continuity restoration from stored state        |
| Operational Trail | Observed continuity evidence across time        |
| Working State     | Minimal active continuity nucleus               |

Stable semantics help reduce continuity drift across long-running work.

---

# Visible Uncertainty

The runtime intentionally allows uncertainty and degraded continuity to remain visible.

Examples may include:

* incomplete operational evidence
* unresolved seams
* missing observed state
* degraded continuity integrity
* low-confidence routing

The runtime prefers:

```text
explicit uncertainty
```

instead of:

```text
fabricated certainty
```

Visible instability is safer than silent continuity corruption.

---

# Continuity Drift

Continuity drift occurs when systems gradually lose stable semantic boundaries.

Examples include:

* summaries replacing evidence
* assumptions becoming indistinguishable from observation
* navigation layers appearing authoritative
* generated interpretation replacing operational grounding

Over time, these distortions compound.

Memex attempts to reduce continuity drift through:

* explicit truth semantics
* operational grounding
* semantic stability
* continuity validation
* visible uncertainty

---

# Failure Philosophy

The runtime intentionally prefers:

```text
hard failure
```

instead of:

```text
silent continuity corruption
```

Examples may include:

* malformed continuity structures
* invalid lineage
* degraded operational evidence
* unstable semantic boundaries
* ambiguous continuity state

Continuity systems become unreliable when instability is hidden.

---

# Closing Perspective

Truth semantics are part of continuity architecture.

Long-running systems become unstable when:

* observation collapses into interpretation
* summaries replace operational grounding
* projections replace source truth
* uncertainty becomes hidden

Memex attempts to preserve continuity by maintaining explicit semantic boundaries between these layers.

At its core:

```text
continuity depends on stable distinctions
```
