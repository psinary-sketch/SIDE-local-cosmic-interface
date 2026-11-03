# SIDE-local-cosmic-interface v0.1

SIDE-local-cosmic-interface compiles adjacent inequalities over the file's own table. Statements at 7a62ced:

    theorem em_ge_weak       : kappa_x100 .electromagnetism ≥ kappa_x100 .weak (SIDELocalCosmicInterface/Basic.lean :73)
    theorem qm_ge_dark       : kappa_x100 .quantum_mechanics ≥ kappa_x100 .dark_sector (SIDELocalCosmicInterface/Basic.lean :79)

The table kappa_x100 is an input. No statement names a physical κ or a local-cosmic boundary.

## Status

| | |
|---|---|
| Toolchain | `leanprover/lean4:v4.29.0-rc8` |
| Mathlib | not required |
| sorry | 0 |
| axioms | 0 |

Companion papers: `LOCAL_COSMIC_INTERFACE_PAPER`, `SYMMETRY_FILTER_PAPER`, `MATTER_AS_ARITHMETIC_v1_0_CONSOLIDATED.md`.

## The gradient

| Channel | κ × 100 |
|---|---|
| electromagnetism | 98 |
| weak | 95 |
| strong | 85 |
| nuclear | 80 |
| gravity | 75 |
| thermodynamics | 70 |
| quantum mechanics | 60 |
| dark sector | 0 |

The gradient descends monotonically. The dark channel is silent (κ = 0).

## What's verified

### §1 — Eight channels
Direct κ × 100 values for each channel.

### §2 — Monotonic descent
- `em_ge_weak`, `weak_ge_strong`, ..., `qm_ge_dark`
- `gradient_range_98`: range = 98

### §3 — The dark channel is silent
- `only_dark_is_silent`: dark_sector is the unique κ = 0 channel

### §4 — P-smooth violation clustering
- Nine bins from electroweak core to dark sector
- `total_violations_five`: 5 violations total
- `bridge_violations_three`: 3 at the neutrino bridge
- `symmetric_cosmic_violations_zero`: 0 in symmetric cosmic
- `dark_violations_two`: 2 in dark sector

### §5 — Neutrino bridge discriminator
- `symmetric_params_bright`: mixing angles at κ = 100
- `broken_params_silent`: mass-squared differences at κ = 0
- `symmetry_discriminates_kappa`: isSymmetric p ↔ neutrino_kappa_x100 p = 100

### §6 — Model comparison under SIDE
- `lambda_CDM_and_programme_pass_S_and_I`
- `CCC_TL_and_MOND_fail_I`

### §8 — Falsification routes
- Four routes catalogued in their own section

## Build

```bash
lake build
```

Self-contained — no Mathlib.

## Federation context

| Kernel | Role for the cosmology constellation |
|---|---|
| SIDE-omega-b | Ω_b = 4/81 |
| SIDE-quaternionic-dark-sector | Dark/visible ratio decomposition |
| SIDE-t7-topology-cmb | Spatial topology prediction |
| SIDE-silence-principle | The κ = 0 dark interface as silent foundation |

## License

CC-BY 4.0.

> Seale, J. Y. (2026). *SIDE-local-cosmic-interface v0.1: The κ Gradient at the Local-Cosmic Boundary.* A PLACE TO STAND Research Programme.

---

`:: → · ← ::`

