# Educators — EXPFACTORY

**Project:** EXPFACTORY  
**Category:** PSYCHOLOGY  
**Upstream:** https://github.com/expfactory/expfactory  
**Pinned commit:** `885b54583b696762782c7580c7d9ceed40278938`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `d58d8b9b155e914c699ed75882ab8f406fce9a84a60f59d714489a30b59da9ab`  
**Date:** October 2026

## Teaching with EXPFACTORY

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `d58d8b9b155e914c699ed75882ab8f406fce9a84a60f59d714489a30b59da9ab` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
