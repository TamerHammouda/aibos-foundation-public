# PHASE-3 NEXT-STEP POLICY

**Status:** Canonical next-step policy  
**Branch:** `phase-3-agent-first`  
**Repo root:** `aibos-foundation-public`  
**Intent:** define the allowed and disallowed next moves from the current green Phase-3 baseline

---

## 1) Policy Context

This policy is anchored to the current green Phase-3 baseline recorded in:

- `/docs/phase3/PHASE-3-GREEN-BASELINE.md`

It exists to keep future work aligned with the current constitutional posture and to prevent execution drift.

This document is descriptive and policy-oriented only. It does not itself authorize execution, minting, resolution, or runtime actuation.

---

## 2) Current Canonical Posture

The current Phase-3 posture remains:

- validation-first
- fail-closed
- execution-neutral
- CI-green on the main validation workflows
- documentation-backed for restart and handoff continuity

Execution remains blocked.

That is the correct baseline.

---

## 3) Allowed Next Work

The following next work is currently allowed:

### A. Documentation-first consolidation
Examples:
- clarifying canonical docs
- tightening handoff docs
- improving coverage indexes
- improving Phase-3 entrypoints
- documenting green baseline implications
- documenting boundaries between proposal / approval / authority / execution

### B. Backward-compatible validation hardening
Examples:
- adding regression runners
- adding validator coverage for already-landed contracts
- improving CI portability for canonical example paths
- improving fail-closed validation messaging
- tightening consistency checks without changing execution posture

### C. Design-only future contract planning
Only if explicitly kept design-only:
- mint-helper proposal design
- future authority-chain design notes
- future resolver design notes
- future consumer design notes

These must remain:
- non-executing
- non-runtime
- non-authorizing
- documentation-first unless validators/tests/CI are explicitly added

---

## 4) Explicitly Disallowed Next Work

The following work is not allowed from this baseline without a later explicit governance decision:

### A. Runtime execution work
Examples:
- enabling execution paths
- implementing live execution gates
- introducing real-world actuation
- adding side-effecting runtime actions

### B. Live token authority operations
Examples:
- live minting
- runtime token issuance
- runtime token consumption
- automatic resolver flows
- revocation engine actuation

### C. Silent semantic drift
Examples:
- changing validator meaning without tests
- changing contract semantics without doc updates
- changing canonical JSON or hash behavior without explicit re-validation
- changing fail-closed behavior without explicit governance review

### D. Multi-change expansion without stabilization
Examples:
- combining architecture work and CI work in one step
- adding new runtime semantics before documenting the current baseline
- broad refactors that weaken traceability

---

## 5) Required Discipline For All Next Work

All next work must preserve:

- fail-closed by default
- proposal ≠ authority ≠ execution
- execution remains blocked unless explicitly enabled by a valid future authority chain
- deterministic canonical JSON + content hash as source-of-truth
- validator/test + CI for every new behavior
- one change at a time:
  - plan
  - diff
  - local checks
  - commit
  - push

This discipline is not optional.

---

## 6) Recommended Immediate Path

From the current green baseline, the recommended immediate path is:

### Preferred
Continue Option A:
- finish documentation consolidation
- strengthen new-chat continuity
- keep repo narration aligned with machine contracts

### Later
Only after Option A feels sufficiently complete:
- consider Option B design-only mint-helper proposal work

### Not now
Do not begin:
- runtime execution work
- live authority-chain implementation
- resolver implementation
- consumer implementation
- actuation-layer work

---

## 7) Summary

This policy freezes the immediate Phase-3 next-step posture.

From the current green baseline:

- documentation-first is allowed
- backward-compatible validation hardening is allowed
- design-only future-contract planning is allowed
- execution-enabling or runtime actuation work is not allowed

Execution remains blocked.

That is the correct policy.
