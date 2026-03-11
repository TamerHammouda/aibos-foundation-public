# PHASE-3 README

**Status:** Canonical Phase-3 entrypoint  
**Branch:** `phase-3-agent-first`  
**Repo root:** `aibos-foundation-public`  
**Intent:** provide a single Phase-3 documentation entrypoint for checkpoint review, green-baseline review, approval-lane review, and future handoff continuity

---

## 1) Primary Phase-3 Canonical Docs

Start here first:

- `/docs/phase3/PHASE-3-CHECKPOINT.md`
- `/docs/phase3/PHASE-3-GREEN-BASELINE.md`

These two files are the main canonical references for:
- current stable posture
- current green baseline
- current next-step discipline

---

## 2) Approval-Lane Canonical Docs

Approval-lane documentation lives under:

- `/docs/approval/README.md`
- `/docs/approval/APPROVAL-COVERAGE-INDEX.md`
- `/docs/approval/CHANGELOG.md`
- `/docs/approval/NEW-CHAT-HANDOFF.md`

These files describe:
- approval-lane scope
- canonical examples
- regression coverage
- historical milestones
- future new-chat continuity

---

## 3) Key Validation / Regression Runners

Important runners and validators include:

### Approval lane
- `/agent/approval/validate_approval_artifact_regressions_ci.py`
- `/agent/approval/validate_approval_decision_bundle_regressions.py`

### Execution-gate vectors
- `/agent/execution/validate_execution_gate_vectors.py`

### Core validation layer
- `/agent/validation/emit_risk_receipt.py`
- `/agent/validation/validate_schema.py`
- `/agent/validation/validate_chain_integrity.py`
- `/agent/validation/validate_test_vectors.py`

### Approval-ledger portability-stabilized validators
- `/agent/ledger/validate_approval_ledger_pack_hash_vectors.py`
- `/agent/ledger/validate_approval_ledger_pack_hash_consistency.py`
- `/agent/ledger/validate_approval_ledger_pack_duplicate_semantics.py`

---

## 4) Current Phase-3 Posture

Phase-3 is currently:

- validation-first
- fail-closed
- execution-neutral
- CI-green on the main validation workflows
- documentation-backed for restart and handoff continuity

Execution remains blocked.

That is the correct posture.

---

## 5) Main Green Workflow Set

The baseline green workflow set is:

- `approval-artifact-ci`
- `execution-gate-vectors-ci`
- `governance-ci`
- `immutability-layer`

Reference:
- `/docs/phase3/PHASE-3-GREEN-BASELINE.md`

---

## 6) Non-Negotiable Invariants

All Phase-3 work must preserve:

- fail-closed by default
- proposal ≠ authority ≠ execution
- execution remains blocked unless explicitly enabled by a valid future authority chain
- deterministic canonical JSON + content hash remain source-of-truth
- every new behavior must ship with validator/test + CI
- one change at a time: plan → diff → local checks → commit → push

---

## 7) Recommended Next-Step Policy

From this Phase-3 entrypoint, the safest next work remains:

- backward-compatible
- validation-first
- execution-neutral
- documentation-first unless a new contract is explicitly being designed

Recommended immediate continuation:
- finish Option A documentation consolidation
- only then consider any design-only mint-helper proposal work

---

## 8) Summary

This file is the single entrypoint for the current canonical Phase-3 state.

For current posture:
- read `/docs/phase3/PHASE-3-CHECKPOINT.md`

For current green baseline:
- read `/docs/phase3/PHASE-3-GREEN-BASELINE.md`

For approval-lane continuity:
- read `/docs/approval/README.md`
