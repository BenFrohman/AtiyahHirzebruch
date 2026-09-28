# Atiyah–Hirzebruch

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
