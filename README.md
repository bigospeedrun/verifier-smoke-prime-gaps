# Verifier smoke fixture: bounded prime gaps

This repository holds the maintainer smoke runs of the `prime-gaps` profile of
https://github.com/bigospeedrun/verifier (board: https://bigospeedrun.com/other/prime-gaps).
It is test data for the verifier, not a new result.

- `main`: `Race.bound : BigOSpeedrun.PrimeGaps.Bound 246`. The proof is darkhipo's composition
  https://github.com/darkhipo/prime-gaps-246-lean at `ac0eb01b6617f5b3bd978037bff937488ad34e73`
  (Apache-2.0), moved into the Submission layout. Its modules are under `Submission/`, its imports
  name `Submission.*`, and no other line changes. The certificate JSON files move with their modules.
  The upstream work: Axiom Math, https://github.com/AxiomMath/PrimeGapsLib at
  `1faa7b14e82ddebc2772dfb9153922f01b106477` (the 246 theory and the 50-tuple certificate), and
  Jonas Whidden (kimihiro64), https://github.com/kimihiro64/bombieri-vinogradov at
  `7a1748306e026825ed6a5555516cc2f28989b2ac` (the Bombieri-Vinogradov theorem), with three
  modules of https://github.com/kimihiro64/Robin1984 at `bfa72aec0c25c8ee29cefe4449d778ff30412bee`.
  The verifier pins PrimeNumberTheoremAnd (kimihiro64 fork `0f15a38c`) and LeanArchitect
  (`d9013cc0`) as solution dependencies.
- Other branches: the statement copy with `sorry` (the control) and statement mutations, each of
  which the verifier must refuse.

License: Apache-2.0 (LICENSE). Attribution of the upstream files: UPSTREAM-NOTICE.md; every
upstream file keeps its own header.
