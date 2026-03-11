# PHASE-3 GREEN BASELINE

**Status:** Canonical green baseline  
**Branch:** `phase-3-agent-first`  
**Repo root:** `aibos-foundation-public`  
**Baseline intent:** record the first fully green Phase-3 validation baseline after approval-lane hardening and CI reconciliation

---

## 1) Baseline State

AI-BOS Phase-3 is currently in a validation-first, execution-neutral, fail-closed posture with the main validation workflows green on `phase-3-agent-first`.

---

## 2) Workflow State

The following workflows are green at this baseline:

- `approval-artifact-ci`
- `execution-gate-vectors-ci`
- `governance-ci`
- `immutability-layer`

This baseline reflects a repo state where approval-lane validation, token-governance validation, immutability checks, and execution-gate vector checks are aligned.

---

## 3) Approval Lane State

The approval lane is now stable and includes:

- canonical approval schemas
- canonical approval examples
- approval artifact regression runner
- approval decision bundle regression runner
- approval coverage index
- approval README
- approval changelog
- approval new-chat handoff

Primary approval docs live under:

- `/docs/approval/`

Primary approval runners live under:

- `/agent/approval/`

---

## 4) Governance / Token State

The token governance stack remains:

- validation-only
- execution-neutral
- fail-closed by default
- deterministic via canonical JSON + content hash
- separated across proposal, approval, authority, and execution semantics

No landed token-layer contract authorizes execution.

---

## 5) Execution State

Execution remains:

- blocked
- constitutionally deny-safe
- not runtime-enabled
- not authority-enabled by default
- not implicitly unlocked by approval artifacts or token contracts

This is the correct and intended state.

---

## 6) What Was Stabilized To Reach Green

This green baseline includes the following stabilization work:

- approval artifact regression coverage in CI
- approval decision bundle regression coverage in CI
- approval-ledger pack-hash validator CI portability
- approval-ledger pack-hash consistency validator CI portability
- approval-ledger duplicate semantics validator CI portability
- governance CI shell parsing fix
- execution-gate vectors CI shell-block cleanup
- execution-gate vectors CI dependency installation fix
- Phase-3 checkpoint refresh with approval-lane status

---

## 7) Non-Negotiable Invariants

This baseline preserves:

- fail-closed by default
- proposal ≠ authority ≠ execution
- execution remains blocked unless explicitly enabled by a valid future authority chain
- deterministic canonical JSON + content hash remain source-of-truth
- every new behavior must ship with validator/test + CI
- one change at a time: plan → diff → local checks → commit → push

---

## 8) Recommended Next-Step Policy

From this baseline, the safest next work should remain:

- backward-compatible
- validation-first
- execution-neutral
- documentation-first unless a new contract is explicitly being designed

Recommended immediate path after this baseline:
- continue Option A documentation consolidation first
- only then consider any design-only mint-helper proposal work

---

## 9) Summary

This document marks the first fully green Phase-3 baseline after approval-lane consolidation and CI reconciliation.

AI-BOS is now in a stable validation-first posture in `aibos-foundation-public` on branch `phase-3-agent-first`.

Execution remains blocked.

That is the correct baseline.
