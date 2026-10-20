# Execution validation

Validated on 2026-10-20 using Python 3.12 on Windows.

- All 32 code cells completed in order in a fresh Python namespace.
- Matplotlib used the non-interactive Agg backend. Selected figures were saved from the notebook's plotting calls.
- The source dataset was freshly downloaded through `kagglehub`; the input had 301 rows.
- No original notebook outputs, machine paths, credentials or raw data are included in this public copy.
- `requirements.txt` pins the eight directly tested analysis packages. JupyterLab is included as the interactive front end; the browser notebook interface was not part of this execution check.

## Observed original-scale scores

| Measure | Value |
|---|---:|
| Training R² | 0.9817 |
| Test R² | 0.9850 |
| Test RMSE | 0.6920 |

These numbers reproduce this exploratory workflow. They are not an independently validated benchmark or classification accuracy. Several regularized fitting calls emitted convergence warnings (423 warning occurrences in this run). Completion does not imply every optimizer fully converged. See the evaluation limitations in the README.

The dataset SHA-256, package versions and machine-readable metrics are recorded in `results/metrics.json`.
