# Seam Model

> Memex State models unresolved boundaries directly.

The runtime refers to these boundaries as:

```text
seams
```

A seam represents the active point where continuity, implementation, reasoning, or system behavior remains unresolved.

---

# Why Seams Exist

Long-running development work rarely fails because information is missing entirely.

More often, work fails because unresolved boundaries become fragmented across:

* conversations
* files
* runtime state
* implementation branches
* undocumented assumptions
* partial decisions

Over time:

* continuity drifts
* priorities blur
* unresolved work becomes hidden
* reasoning fragments

Memex attempts to reduce this fragmentation by treating unresolved boundaries as explicit runtime state.

---

# What a Seam Represents

A seam is:

```text
an active unresolved boundary
```

Examples include:

* architectural uncertainty
* unstable runtime behavior
* incomplete integrations
* unresolved protocol transitions
* ambiguous implementation boundaries
* continuity mismatches
* validation failures
* routing uncertainty

A seam does not need to represent failure.

It represents:

```text
active unresolved state
```

---

# Seam vs Task

A seam is not the same thing as a task.

Tasks describe:

* work items
* actions
* objectives
* deliverables

Seams describe:

* unresolved boundaries
* instability surfaces
* continuity pressure points
* active system tension

Example:

| Type | Example                                                             |
| ---- | ------------------------------------------------------------------- |
| Task | Add snapshot export retry handling                                  |
| Seam | Snapshot persistence reliability during degraded runtime conditions |

Tasks may change rapidly.

The seam often persists across multiple implementation steps.

---

# Seam vs Bug

A seam is also not the same thing as a bug.

A bug is usually:

* localized
* observable
* directly fixable

A seam may involve:

* incomplete understanding
* evolving architecture
* uncertain system boundaries
* multiple interacting systems
* unresolved operational behavior

Some seams eventually produce bugs.

Some bugs reveal deeper seams.

---

# Current Seam

Memex preserves a canonical:

```text
current_seam
```

This represents the active unresolved boundary at the current point in runtime continuity.

The current seam acts as a continuity anchor.

It helps preserve:

* implementation focus
* architectural context
* runtime trajectory
* unresolved system pressure

across sessions.

---

# Next Action

The runtime also preserves:

```text
next_action
```

The next action represents:

```text
the immediate move applied to the current seam
```

The runtime intentionally separates:

* unresolved boundaries
* from
* actions applied to those boundaries

---

# Semantic Separation

The runtime explicitly enforces:

```text
current_seam != next_action
```

This exists because:

* the seam is the unresolved condition
* the action is the response applied to it

Collapsing these into the same value weakens continuity clarity.

---

# Seam Persistence

Seams often persist across multiple sessions.

Examples:

* runtime stability work
* protocol redesign
* continuity validation
* repository reliability
* operational integrity

The runtime treats seams as continuity-level state instead of session-local notes.

---

# Seam Trajectory

Memex also tracks:

```text
recent seams
```

This exists to preserve short-term continuity trajectory.

The goal is to reduce:

* tunnel vision
* isolated implementation focus
* context collapse
* fragmented reasoning

A project may move through multiple related seams over time.

Tracking seam trajectory helps preserve awareness of how the system evolved.

---

# Seam-Centered Resume

During resume flows, seams help reconstruct:

* active architectural pressure
* unresolved implementation boundaries
* runtime instability surfaces
* current continuity focus

This allows resume state to preserve:

```text
why work is happening
```

instead of only:

```text
what files changed
```

---

# Seams and Repository Navigation

Repository navigation systems may use the current seam to help surface:

* relevant files
* related implementation surfaces
* nearby repository context
* unresolved implementation areas

This navigation remains advisory.

The seam does not override source truth.

---

# Seam Stability

A seam should remain semantically stable long enough to preserve continuity.

Examples of weak seams:

* vague implementation tasks
* temporary todos
* highly volatile wording
* ambiguous objectives

Examples of stronger seams:

* protocol boundary instability
* runtime validation mismatch
* continuity drift
* operational integrity uncertainty

The runtime benefits when seams represent meaningful unresolved system boundaries.

---

# Design Philosophy

Memex models seams directly because:

```text
long-running systems accumulate unresolved boundaries
```

If those boundaries remain implicit:

* continuity drifts
* reasoning fragments
* implementation loses direction
* architectural pressure becomes invisible

Explicit seams help preserve continuity shape over time.

---

# Closing Perspective

The seam model exists to make unresolved system boundaries visible.

Instead of treating continuity as:

* disconnected sessions
* isolated tasks
* fragmented implementation steps

Memex attempts to preserve:

* active boundaries
* continuity pressure
* runtime trajectory
* unresolved system state

across long-running AI-assisted work.
