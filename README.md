# Daniel Rosenbluth

Daniel Rosenbluth is an inventor and IP author whose primary work is VaultGhost — a forensic, recursive method for tracing prompt influence, latent drift, and linguistic pattern replication across LLM systems. A U.S. provisional patent was filed February 25, 2026. The underlying protocol and verification infrastructure are built and maintained here as a protocol engineer.

---

## What VaultGhost Is

VaultGhost is a forensic, recursive method for tracing prompt influence, latent drift, and linguistic pattern replication across LLM systems. It combines Ed25519 digital signatures with JCS canonicalization to produce verifiable, tamper-evident records of model behavior. The chain ledger tracks SHA-256 artifact provenance across runs, with honest documentation of chain breaks rather than suppression of them. The protocol is spec-driven: what is implemented and what is only specified are kept distinct.

---

## Where to Start

1. [**vaultghost-protocol**](https://github.com/drosenbluth25/vaultghost-protocol) — Canonical technical reference. VaultGhost Protocol v1.1.1 FINAL-2.2, Apache-2.0, with CITATION.cff for academic citation.
2. [**spec-orchestration-eval-harness**](https://github.com/drosenbluth25/spec-orchestration-eval-harness) — Reproducible eval harness for spec-driven LLM orchestration benchmarking; the primary public bridge artifact.
3. [**vaultghost-verify**](https://github.com/drosenbluth25/vaultghost-verify) — Deterministic verification pipeline (`make verify`, `EXPECTED_OUTPUT.txt`, non-zero exit on failure).
4. [**vaultghost-chain-ledger**](https://github.com/drosenbluth25/vaultghost-chain-ledger) — SHA-256 artifact provenance chain, including documented chain break RUN-008 MISSING.

---

## Implementation Status

| Repo | Status |
|---|---|
| [vaultghost-core](https://github.com/drosenbluth25/vaultghost-core) | Implemented |
| [vaultghost-verify](https://github.com/drosenbluth25/vaultghost-verify) | Implemented |
| [vaultghost-chain-ledger](https://github.com/drosenbluth25/vaultghost-chain-ledger) | Implemented |
| [vaultghost-stub](https://github.com/drosenbluth25/vaultghost-stub) | Implemented (Python + Rust) |
| [vaultghost-protocol](https://github.com/drosenbluth25/vaultghost-protocol) | Specified |
| [spec-orchestration-eval-harness](https://github.com/drosenbluth25/spec-orchestration-eval-harness) | Implemented (private) |

---

## Public Landing Page

[drosenbluth25.github.io](https://drosenbluth25.github.io)

---

Serious build phase began January 2026; the account dates to 2022.
