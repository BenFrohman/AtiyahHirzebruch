# Statement

## Integral Hodge conjecture (false)

Every class in `H^{2k}(X,Z) ∩ H^{k,k}(X)` is the class of an integral algebraic cycle.

**False.** Two independent families:

1. **Torsion** — Atiyah–Hirzebruch 1962. This repo.
2. **Non-torsion** — Kollár 1990/92, very general degree-125 hypersurface in `P^4`. See sister notes.

## Rational Hodge conjecture (Clay, open)

Every class in `H^{2k}(X,Q) ∩ H^{k,k}(X)` is a rational combination of algebraic cycles.

Neither family above inhabits that negation. Torsion dies over `Q`. Kollár's `α` becomes a rational multiple of a hyperplane power.

## Type split on `V(F)`

```
NL_alg :  Σ z, cl(z) = γ
CE     :  Π z, (cl(z) = γ → False)
```

`cl(Π) = [Π]` inhabits `NL_alg` for `γ = [Π]`. Therefore `CE` for that `γ` is empty: a map from an inhabited type to `False` does not exist.

`β = h^2 - 6[Π]` is the integral primitive class in the same span. It is an integral cycle. It is not an integral miss and not a rational miss.
