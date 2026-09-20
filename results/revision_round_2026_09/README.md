# September 2026 reviewer-round results

This directory contains **compact numerical outputs** from the reviewer-driven analyses archived under `notebooks/revision_round_2026_09/`.

These files are included so that a reviewer can audit the numerical claims added during revision **without rerunning every expensive TensorFlow fit**. Large OOF prediction matrices, checkpoint files, bootstrap replicate archives, and redundant figure exports remain excluded to keep the repository compact.

## Included evidence

- `NB11/` — pooled CNN1D performance.
- `NB12/` — whole-egg bootstrap confidence intervals and paired Wilcoxon/Holm comparisons for the seven-model benchmark.
- `NB15/` — unified CPU-only latency/throughput/complexity benchmark.
- `NB16/` — CNN1D, CNN1D-FLAT and CNN1D-GAP+position performance; row-level leakage sensitivity; multi-permutation wavelength-order summaries.
- `NB18/` — calibration slopes, phase-wise MAE/bias/tolerance, and chronological phase-classification summaries.
- `NB19/` — learning curves for 6, 12, 18 and 24 outer-training eggs, relative improvements, and gaps to SVR.

## Scientific status

These analyses were performed after the NB01–NB08 primary workflow and its main egg-disjoint OOF predictions were frozen. They are complementary, diagnostic, sensitivity, or reviewer-requested analyses and **do not retroactively redefine primary model selection**.

The independent biological unit remains the egg. Row-level analyses are intentionally leaky diagnostics only. Learning-curve results are interpreted only over the observed 6–24 training-egg range and are not extrapolated beyond 24 eggs. CPU latencies are environment-specific reference values, not mobile/SCiO deployment timings.

See `notebooks/revision_round_2026_09/README.md` and `docs/MANUSCRIPT_REPOSITORY_MAPPING.md`.
