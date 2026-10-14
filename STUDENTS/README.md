# Students — EXPFACTORY

**Project:** EXPFACTORY  
**Category:** PSYCHOLOGY  
**Upstream:** https://github.com/expfactory/expfactory  
**Pinned commit:** `885b54583b696762782c7580c7d9ceed40278938`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `d58d8b9b155e914c699ed75882ab8f406fce9a84a60f59d714489a30b59da9ab`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `885b54583b696762782c7580c7d9ceed40278938`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `d58d8b9b155e914c699ed75882ab8f406fce9a84a60f59d714489a30b59da9ab`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
