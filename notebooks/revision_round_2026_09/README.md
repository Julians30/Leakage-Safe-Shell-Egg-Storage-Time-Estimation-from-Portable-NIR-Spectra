# Revision-round notebooks (September 2026)

These notebooks document analyses added during peer review **after** the NB01–NB08 primary workflow and its main egg-disjoint OOF predictions had been frozen. They are complementary, sensitivity, diagnostic, or presentation analyses and do not redefine the primary validation design.

## Execution / provenance map

| Stage | Notebook | Role |
|---|---|---|
| NB05B | `NB05B_MULTISEED_SHUFFLE_ABLATION.ipynb` | Four additional target-independent wavelength shuffles, extending the original-order ablation to five permutations. |
| NB09A | `NB09A_ROW_LEVEL_LEAKAGE_DIAGNOSTIC.ipynb` | Deliberately leaky row-level partition diagnostic used only to quantify optimism from biological-unit overlap. |
| NB09B | `NB09B_REVIEWER_ADDITIONAL_ANALYSES_OPTIMIZED.ipynb` | Wider-grid SVR sensitivity, storage-age phase summaries, attenuation diagnostics, and reviewer-requested supporting analyses. |
| NB10 | `NB10_REVISED_PUBLICATION_FIGURES.ipynb` | Revised publication figures derived from frozen outputs. |
| NB11 | `NB11_CNN1D_REVIEWER_BENCHMARK.ipynb` | Compact 1D-CNN benchmark under the same egg-disjoint protocol. |
| NB12 | `NB12_CLUSTERED_UNCERTAINTY_AND_INFLUENCE.ipynb` | Whole-egg bootstrap uncertainty, paired inference, fold heterogeneity, and leave-one-egg influence diagnostics. |
| NB13 | `NB13_REVIEWER_TABLES_FIGURES.ipynb` | Reviewer-facing summary tables and diagnostic figures. |
| NB14 | `NB14_FINAL_RESULTS_PACKAGE.ipynb` | Integrity audit and packaging of the first reviewer-round result bundle. |
| NB15 | `NB15_UNIFIED_COMPUTATIONAL_BENCHMARK_v6.ipynb` | Unified CPU-only computational benchmark and Figure 6 generation. |
| NB16 | `NB16_CNN1D_POSITION_AWARE_SENSITIVITY.ipynb` | Position-aware CNN1D variants, row-level sensitivity, and convolutional wavelength-order ablation. |
| NB18 | `NB18_CALIBRATION_PHASES_AND_SVR_SURFACE.ipynb` | Calibration slopes/curves, phase-wise and day-wise error structure, and SVR error-surface diagnostics. |
| NB19 | `NB19_LEARNING_CURVE.ipynb` | Learning curves at 6, 12, 18, and 24 outer-training eggs using frozen configurations. |

There is intentionally **no NB17** in the final revision sequence.

## NB15 provenance note

The reported numerical computational package was produced under run revision
`NB15_v5_three_path_cpu_latency_plus_figure6`. The exact executed v5 notebook is retained under
`archive/NB15_UNIFIED_COMPUTATIONAL_BENCHMARK_v5_EXECUTED.ipynb`.

The public v6 notebook changes only the documentation and a small Figure 6 label offset for ANN to avoid text overlap on some Colab CPU assignments. It does not alter predictive metrics, OOF predictions, statistical tests, or the timing protocol.

## Interpretation guardrails

- The egg remains the independent biological unit.
- Outer-test eggs are not used for model/preprocessing/epoch selection.
- Post hoc analyses are identified as such and do not replace the frozen primary estimates.
- Row-level splitting is intentionally leaky and diagnostic only.
- Deep-learning seeds are algorithmic repeats, not biological replicates.
- Learning curves do not support extrapolation beyond 24 training eggs.
- CPU latency values are environment-specific engineering references, not SCiO/mobile deployment timings.
