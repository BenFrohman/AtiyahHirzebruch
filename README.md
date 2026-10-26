<!-- Copyright (c) 2026 Benjamin Stanley Frohman. Licensed under Apache-2.0. -->
# Atiyah–Hirzebruch

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23652971.svg)](https://doi.org/10.5281/zenodo.23652971) [![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

**Status:** literature counterexample to the *integral* Hodge conjecture.
**Not** a counterexample to Clay rational Hodge.
**Author:** Benjamin Stanley Frohman (@BenFrohman)
**License:** Apache-2.0. © 2026 Benjamin Stanley Frohman.

This shelf records one of the two classical counterexamples to

```
CH^k(X) → H^{2k}(X,Z) ∩ H^{k,k}(X)
```

being surjective. The other shelf is Kollár (non-torsion). Neither shelf is Term B of rational Hodge.

## The theorem (Atiyah–Hirzebruch 1962)

There exist smooth complex projective varieties and torsion classes

```
α ∈ H^{2k}(X,Z) ∩ H^{k,k}(X),    nα = 0 for some n > 0,
```

that are not the class of an algebraic cycle.

Source: M. F. Atiyah and F. Hirzebruch, *Analytic cycles on complex manifolds*, Topology 1 (1962), 25–45.

Totaro (1997) recast the same examples in complex cobordism: the refined cycle class `CH^*(X) → MU^*(X) ⊗_{MU_*} Z` misses those torsion classes.

## Why this is not Clay

Clay Hodge is the *rational* statement:

```
H^{2k}(X,Q) ∩ H^{k,k}(X)  =  im( cl : CH^k(X)_Q → H^{2k}(X,Q) ).
```

A torsion class dies after `⊗ Q`. If `nα = 0` in integral cohomology, then `α = 0` in rational cohomology. An Atiyah–Hirzebruch class is therefore invisible to the Clay map. It cannot inhabit

```
CE = ⟨ X, γ, miss_γ ⟩
```

with `γ` a rational Hodge class.

## Sister statement (not this repo)

Kollár produced *non-torsion* integral Hodge classes that are still not algebraic: a very general hypersurface of degree 125 in `P^4` carries a class `α` of degree 1 whose every algebraic curve has degree divisible by 5. Then `5α` is algebraic and `α` is not. After `⊗ Q` the class is a multiple of the hyperplane power, so rational Hodge on that threefold is Lefschetz and holds.

## What this repo does not contain

- a term of `Hodge_disproof` / `ClayDisproofTerm`
- a named miss class on `V(F)`
- a proof that `1751 - 2` counts non-algebraic rational classes

`V(F)` and `α = [Π] - (1/6)h^2` are algebraic over `Q`. They live in `NL_alg`, not in `CE`.

---
## Archival DOI & Cryptographic Provenance

- **Dedicated 1-to-1 Zenodo DOI:** [10.5281/zenodo.23652971](https://doi.org/10.5281/zenodo.23652971)
- **Author:** Benjamin Stanley Frohman (ORCID: [0009-0006-7068-3718](https://orcid.org/0009-0006-7068-3718))
- **License:** Apache License, Version 2.0 (`Copyright (c) 2026 Benjamin Stanley Frohman`)
- **Earliest Commit Provenance:** `4324e2550e8982bf1555a837ef0ead5957e00e26` (2026-09-28 06:55:02 PM CDT (UTC-5))
- **SealGuard SHA-256 Merkle Root:** `a054ea4d7be2498d849264414e85a499f1a48067ff23f8d6572fd610e15680ce` (`PROVENANCE_MERKLE_ROOT.json`)
- **Titan Audit Certificate:** `audit/TITAN_AUDIT_CERTIFICATE.json` (Ed25519 key `b428fb72676f1c52`)
- **Scope & Scientific Boundary:** This repository records known 1962 integral torsion obstructions (Atiyah-Hirzebruch) and their vanishing after rationalization. It does not prove or disprove the rational Clay Hodge Conjecture.
