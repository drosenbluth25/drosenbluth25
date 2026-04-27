# Daniel Rosenbluth

Daniel Rosenbluth is a protocol engineer and IP author. The primary work is **VaultGhost** — an independent evidence-layer protocol for AI interaction provenance, attribution, and auditability. A U.S. provisional patent was filed February 25, 2026. The protocol and its verification infrastructure are designed, specified, and maintained here.

---

## What VaultGhost Is

VaultGhost is an independent evidence-layer protocol for AI interaction provenance, attribution, and auditability. It focuses on captured-boundary records: prompts, outputs, metadata, hashes, signatures, schemas, verification results, and reproducible audit artifacts. The protocol does not claim access to hidden model states or provider-internal systems. Its purpose is to make AI-mediated interactions more verifiable, replayable, and tamper-evident.

In practice this means:

- **Captured-boundary records.** Prompts, outputs, and associated metadata are recorded at the user/model boundary.
- **Cryptographic integrity.** Ed25519 digital signatures over JCS-canonicalized JSON; SHA-256 hashing of artifacts.
- **Chain provenance.** A run-by-run artifact ledger that links records by hash, with chain breaks documented explicitly rather than suppressed.
- **Spec-driven distinction.** What is **implemented**, what is only **specified**, what is **experimental**, and what is **archival** are kept clearly separated.

---

## Where to Start

1. [**vaultghost-protocol**](https://github.com/drosenbluth25/vaultghost-protocol) — Canonical formal specification (`SPECIFICATION.md`). Apache-2.0. Includes `CITATION.cff` for academic citation.
2. [**vaultghost-core**](https://github.com/drosenbluth25/vaultghost-core) — Reference Python core library and schemas.
3. [**vaultghost-verify**](https://github.com/drosenbluth25/vaultghost-verify) — Deterministic verification pipeline (`make verify`, `EXPECTED_OUTPUT.txt`, non-zero exit on failure).
4. [**vaultghost-chain-ledger**](https://github.com/drosenbluth25/vaultghost-chain-ledger) — SHA-256 artifact provenance chain, including documented chain-break record `RUN-008 MISSING`.

For the full repo map, including private and archival repos, see [`REPOS.md`](REPOS.md).

---

## Implementation Status

Statuses follow the legend used in [`REPOS.md`](REPOS.md): **Implemented**, **Specified**, **Experimental**, **Archival**, **Private/Internal**.

| Repo | Status | Visibility |
|---|---|---|
| [vaultghost-core](https://github.com/drosenbluth25/vaultghost-core) | Implemented | Public |
| [vaultghost-verify](https://github.com/drosenbluth25/vaultghost-verify) | Implemented | Public |
| [vaultghost-chain-ledger](https://github.com/drosenbluth25/vaultghost-chain-ledger) | Implemented | Public |
| [vaultghost-stub](https://github.com/drosenbluth25/vaultghost-stub) | Implemented (Python + Rust) | Public |
| [vaultghost-protocol](https://github.com/drosenbluth25/vaultghost-protocol) | Specified | Public |
| spec-orchestration-eval-harness | Implemented | Private/Internal |

---

## Public Landing Page

[drosenbluth25.github.io](https://drosenbluth25.github.io)

---

## Notes

- License terms vary by repository. The protocol specification (`vaultghost-protocol`) is released under Apache-2.0; the reference stub (`vaultghost-stub`) is CC0. Other repos carry their own licenses where present. This profile repository itself does not currently carry a `LICENSE` file — license decision required.
- Serious build phase began January 2026; the GitHub account dates to 2022.
