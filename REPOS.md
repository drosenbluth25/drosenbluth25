# VaultGhost Ecosystem — Repo Map

**GitHub org/user:** [drosenbluth25](https://github.com/drosenbluth25)

> Private repos are listed for completeness but are not publicly accessible. Their descriptions are derived from available metadata and task specification.

---

## Legend

| Status | Meaning |
|---|---|
| **Implemented** | Code is present and functional |
| **Specified** | Spec exists; implementation is partial or private |
| **Experimental** | In active development; not stable |
| **Archival** | Historical record; not actively developed |
| **Private/Internal** | Exists but not public |

---

## Start Here

| Repo | Status | Visibility | Notes |
|---|---|---|---|
| [drosenbluth25.github.io](https://github.com/drosenbluth25/drosenbluth25.github.io) | — | Public | Ecosystem landing page and archive index |

---

## Core Protocol

| Repo | Status | Visibility | Notes |
|---|---|---|---|
| [vaultghost-protocol](https://github.com/drosenbluth25/vaultghost-protocol) | Specified | Public | Canonical formal specification (`SPECIFICATION.md`), Apache-2.0; implementation lives in companion repos |
| [vaultghost-core](https://github.com/drosenbluth25/vaultghost-core) | Implemented | Public | Python core library; `schemas/` and `vaultghost_core/` package |
| on-ledger-registry-spec | Specified | Private | On-ledger versioning and registry specification |
| vaultghost-rfc | Specified | Private | RFC-style protocol change proposals |

---

## Verification

| Repo | Status | Visibility | Notes |
|---|---|---|---|
| [vaultghost-verify](https://github.com/drosenbluth25/vaultghost-verify) | Implemented | Public | Deterministic `make verify` pipeline; hash-chain validation and receipt matching |

---

## Chain Ledger / Provenance

| Repo | Status | Visibility | Notes |
|---|---|---|---|
| [vaultghost-chain-ledger](https://github.com/drosenbluth25/vaultghost-chain-ledger) | Implemented | Public | Byte-level run artifacts and `CHAIN_INDEX.json`; honest chain-break documentation |
| VaultGhost-Forensic-Attribution-Protocol | Specified | Private | Forensic attribution spec layered over the chain ledger |

---

## Turn Records / Stubs / Integrations

| Repo | Status | Visibility | Notes |
|---|---|---|---|
| [vaultghost-turn-records](https://github.com/drosenbluth25/vaultghost-turn-records) | Archival | Public | Cross-platform turn records (Perplexity + Grok) with OpenTimestamps Bitcoin anchoring |
| [vaultghost-stub](https://github.com/drosenbluth25/vaultghost-stub) | Implemented | Public | Reference implementation stub (Python + Rust); red-team review target, CC0 |
| vaultghost-integration | Experimental | Private | Integration layer; active development, not stable |

---

## Evaluation Harness

| Repo | Status | Visibility | Notes |
|---|---|---|---|
| spec-orchestration-eval-harness | Implemented | Private | Orchestration evaluation harness against protocol spec |

---

## Archival / Reference

| Repo | Status | Visibility | Notes |
|---|---|---|---|
| ProvenanceSync-3.2-Capsule | Archival | Private | Versioned provenance snapshot; historical reference capsule |
| perplexity-model-watcher | Archival | Private | Historical record of model behavior observations |
| [David-Passon](https://github.com/drosenbluth25/David-Passon) | Archival | Public | Minimal public repo; single commit, no active development |
