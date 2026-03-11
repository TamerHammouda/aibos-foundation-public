# PUBLIC SCOPE

**Status:** Public mirror policy  
**Public repo:** `aibos-foundation-public`  
**Private source repo:** `/Users/tamerhamouda/AI-Boss/aibos`  
**Intent:** define what content may be published in the public mirror and what content must remain private

---

## 1) Purpose

This repository is a curated public mirror of selected AI-BOS foundation materials.

It is **not** the source-of-truth working repository.

The private repository at:

`/Users/tamerhamouda/AI-Boss/aibos`

remains the canonical implementation and governance source.

---

## 2) Public Mirror Principles

This public repository is:

- curated
- documentation-first
- governance-oriented
- execution-neutral
- manually published

This public repository is **not**:

- an automatic mirror
- a runtime repository
- an implementation repository
- an authority-issuing repository
- an execution-enabled repository

---

## 3) Allowed In Public

The following content types are generally allowed in this public mirror:

- high-level architecture documentation
- phase summaries
- checkpoints
- green baseline documentation
- roadmap-style docs
- public-safe design-only conceptual docs
- changelogs
- handoff docs
- indexes and glossaries
- sanitized diagrams
- public-safe examples that do not imply execution or authority

---

## 4) Private By Default

The following content types remain private by default and should not be published here unless explicitly reviewed and sanitized:

- anything under `audit/`
- secrets, tokens, credentials, keys, or environment-specific values
- internal-only workflow mechanics
- sensitive CI details
- machine-specific paths
- runtime execution logic
- minting logic
- resolver logic
- consumer logic
- private operational details
- sensitive governance enforcement details
- unsanitized machine contracts
- implementation artifacts that increase attack surface

---

## 5) Review-Required Content

The following categories require deliberate review before any public release:

- schemas
- validators
- CI workflow files
- regression runners
- machine-readable governance contracts
- approval-lane machine artifacts
- authority-lane machine artifacts
- execution-adjacent examples
- examples that may be misunderstood as real authority or execution artifacts

If there is doubt, the content stays private.

---

## 6) Publication Rule

Before publishing any file to this mirror, apply this test:

**If this file were permanently public, forked, copied, indexed, and quoted, would it still be safe and acceptable?**

If the answer is not a clear yes, it must remain private.

---

## 7) Canonical Source Rule

The private repository remains the source-of-truth for:

- implementation
- validators
- schemas
- CI
- runtime behavior
- governance enforcement
- machine contracts
- active development workflow

The public mirror is only a selective documentation surface.

---

## 8) Execution Posture

Nothing published in this repository should be interpreted as:

- execution authorization
- authority issuance
- minting readiness
- runtime enablement
- implementation approval

Execution remains blocked in the represented posture.

---

## 9) Change Discipline

Changes to this public mirror should be:

- small
- deliberate
- reviewed for public safety
- manually selected
- consistent with the private source repo’s intended public boundary

This repository should never become a blind second copy of the private repo.

---

## 10) Summary

This repository is a curated public-safe window into selected AI-BOS foundation materials.

It is not the implementation repo.

It is not the runtime repo.

It is not the source-of-truth.

The private repository remains canonical.
