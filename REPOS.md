# VaultGhost Ecosystem — Repo Map

**GitHub org/user:** [drosenbluth25](https://github.com/drosenbluth25)

VaultGhost is an independent evidence-layer protocol for AI interaction provenance, attribution, and auditability. It focuses on captured-boundary records: prompts, outputs, metadata, hashes, signatures, schemas, verification results, and reproducible audit artifacts. The protocol does not claim access to hidden model states or provider-internal systems. Its purpose is to make AI-mediated interactions more verifiable, replayable, and tamper-evident.

> Private repos are listed for completeness but are not publicly accessible. They appear as plain text (no link). Their purposes are derived from available metadata and protocol specification.

---

## Legend

| Status | Meaning |
|---|---|
| **Implemented** | Code is present and functional |
| **Specified** | Spec exists; implementation is partial, pending, or private |
| **Experimental** | In active development; not stable |
| **Archival** | Historical record; not actively developed |
| **Private/Internal** | Exists but not public |

---

## Start Here

| Repo | Status | Visibility | Purpose | Notes |
|---|---|---|---|---|
| [drosenbluth25.github.io](https://github.com/drosenbluth25/drosenbluth25.github.io) | Implemented | Public | Ecosystem landing page | Archive index for the public repos |

---

## Core Protocol

| Repo | Status | Visibility | Purpose | Notes |
|---|---|---|---|---|
| [vaultghost-protocol](https://github.com/drosenbluth25/vaultghost-protocol) | Specified | Public | Canonical formal specification | `SPECIFICATION.md`; Apache-2.0; `CITATION.cff` present |
| [vaultghost-core](https://github.com/drosenbluth25/vaultghost-core) | Implemented | Public | Reference Python core library | `schemas/` and `vaultghost_core/` package |
| on-ledger-registry-spec | Specified | Private/Internal | On-ledger versioning and registry specification | Not publicly accessible |
| vaultghost-rfc | Specified | Private/Internal | RFC-style protocol change proposals | Not publicly accessible |

---

## Verification

| Repo | Status | Visibility | Purpose | Notes |
|---|---|---|---|---|
| [vaultghost-verify](https://github.com/drosenbluth25/vaultghost-verify) | Implemented | Public | Deterministic verification pipeline | `make verify`; hash-chain validation and receipt matching; non-zero exit on failure |

---

## Chain Ledger / Provenance

| Repo | Status | Visibility | Purpose | Notes |
|---|---|---|---|---|
| [vaultghost-chain-ledger](https://github.com/drosenbluth25/vaultghost-chain-ledger) | Implemented | Public | SHA-256 artifact provenance chain | Byte-level run artifacts and `CHAIN_INDEX.json`; documented chain-break record `RUN-008 MISSING` |
| VaultGhost-Forensic-Attribution-Protocol | Specified | Private/Internal | Forensic attribution specification layered over the chain ledger | Not publicly accessible |

---

## Turn Records / Stubs / Integrations

| Repo | Status | Visibility | Purpose | Notes |
|---|---|---|---|---|
| [vaultghost-turn-records](https://github.com/drosenbluth25/vaultghost-turn-records) | Archival | Public | Cross-platform captured-boundary turn records | Historical turn-record fixtures; placeholder/simulated timestamp material; no verified anchoring claim. |
| [vaultghost-stub](https://github.com/drosenbluth25/vaultghost-stub) | Implemented | Public | Reference implementation stub | Reference/stub repository; license decision pending because no LICENSE file is currently present. |
| vaultghost-integration | Experimental | Private/Internal | Integration layer | Active development; not stable |

---

## Evaluation Harness

| Repo | Status | Visibility | Purpose | Notes |
|---|---|---|---|---|
| spec-orchestration-eval-harness | Implemented | Private/Internal | Reproducible eval harness for spec-driven LLM orchestration benchmarking | Not publicly accessible |

---

## Archival / Reference

| Repo | Status | Visibility | Purpose | Notes |
|---|---|---|---|---|
| ProvenanceSync-3.2-Capsule | Archival | Private/Internal | Versioned provenance snapshot | Historical reference capsule |
| perplexity-model-watcher | Archival | Private/Internal | Historical record of model behavior observations | Captured-boundary observations only; no provider-internal access |
| [David-Passon](https://github.com/drosenbluth25/David-Passon) | Archival | Public | Minimal public repo | Single commit; no active development |

---

## Licensing Note

License terms vary by repository:

- `vaultghost-protocol` — Apache-2.0
- `vaultghost-stub` — reference/stub repository. Its README previously referenced CC0 intent, but no LICENSE file is currently present; license decision remains pending until owner confirmation.
- Other repos carry their own licenses where present

This profile repository itself does not currently carry a `LICENSE` file — license decision required.

## Patent Note

A U.S. provisional patent was filed **February 25, 2026** covering aspects of VaultGhost. This is a factual filing record only; no claim is made here as to the eventual scope, grant, or enforceability of any resulting patent.
