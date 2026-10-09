[README.md](https://github.com/user-attachments/files/33251231/README.md)
# fv-notebook

A learning notebook for formally verified cryptography: specs in Lean, protocol models in ProVerif, and small Rust code checked against the specs. Public learning material only. Nothing proprietary goes in this repo.

**Status:** Stage 1 of 6 &nbsp;|&nbsp; **Last updated:** 2026/09/9

## Stages

| Stage | Folder | Deliverable | Status |
| --- | --- | --- | --- |
| 1. Security notions | `stage1-notes/` | One page: assumptions of my QKD key delivery | not started |
| 2. Logic and Lean basics | `stage2-lean/` | About 20 proved lemmas, notes on which tactic solved what | not started |
| 3. ML-KEM maths | `stage3-ntt/` | Python NTT checked against schoolbook multiplication | not started |
| 4. First spec | `stage4-spec/` | Lean spec of encode/decode and NTT, run against official test vectors | not started |
| 5. ProVerif | `stage5-proverif/` | Hybrid PQC + QKD handshake model with queries and attack traces | not started |
| 6. Rust | `stage6-rust/` | Small crate whose outputs match the Stage 4 spec | not started |

Status values: `not started`, `in progress`, `check passed` (the stage's readiness check from the guide).

## What is proved, tested and assumed

| Item | Proved | Tested only | Assumed | Notes |
| --- | --- | --- | --- | --- |
| _example: encode/decode round trip_ | yes, for inputs in the stated domain | official vectors | none | `#print axioms` output recorded in `stage4-spec/AXIOMS.md` |

## Open questions and gaps

Things I do not understand yet, with a plan for each.

## Reproducing

Pinned toolchains:

- Lean: see `lean-toolchain` in each Lean folder.
- Rust: see `Cargo.lock` and `rust-toolchain.toml` in `stage6-rust/`.
- ProVerif: version recorded in `stage5-proverif/README.md`.

Build and check everything locally:

```
scripts/check.sh
```

## Trusted base

List what a reader has to trust for the proofs here to mean anything: Lean's kernel, the Lean version, any extraction tool, any axiom used. Keep this section current.

## Log


