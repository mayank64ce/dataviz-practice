# dataviz-practice
A structured tutorial for making publication-quality research figures — the kind you see from top ML labs — using `matplotlib` and `seaborn`. Powered by Claude.

## Goal
Go from zero matplotlib knowledge to producing paper-ready figures for ML research: training curves, model comparisons, distributions, multi-panel layouts, and proper export.

## Stack
- Python (d2l conda environment)
- `matplotlib` 3.7 · `seaborn` 0.13 · `numpy` · `pandas`

## Notebooks

Each notebook is a **guided exercise**: concepts are explained, then you fill in the code yourself.

| # | Notebook | Topics |
|---|----------|--------|
| 01 | [`01_foundations.ipynb`](01_foundations.ipynb) | OO API vs pyplot · Figure/Axes hierarchy · spines · grid · fonts · before/after |
| 02 | [`02_style_system.ipynb`](02_style_system.ipynb) | `rcParams` · style dict · `.mplstyle` file · `rc_context` overrides |
| 03 | [`03_color.ipynb`](03_color.ipynb) | Categorical / sequential / diverging palettes · Okabe-Ito · colorblind safety · color cycles |
| 04 | [`04_training_curves.ipynb`](04_training_curves.ipynb) | Mean ± std bands · multi-run comparison · EMA smoothing · log scale · annotations |
| 05 | [`05_comparisons.ipynb`](05_comparisons.ipynb) | Bar charts · error bars · grouped bars · horizontal bars · lollipop plots |
| 06 | [`06_distributions.ipynb`](06_distributions.ipynb) | Box · violin · strip · KDE · ECDF · layered violin+strip |
| 07 | [`07_multi_panel.ipynb`](07_multi_panel.ipynb) | `GridSpec` · shared axes · panel labels (A/B/C) · arrow annotations · capstone figure |
| 08 | [`08_export.ipynb`](08_export.ipynb) | PDF vs PNG · `savefig` params · venue column widths · reproducible scripts · LaTeX integration |

## Quick start
```bash
conda activate d2l
jupyter notebook 01_foundations.ipynb
```

## Recommended order
Work through notebooks 01 → 08 in sequence. Each notebook builds on the previous:
- Notebook 02 uses the `clean_axes` helper from 01
- Notebooks 03–08 all load `research.mplstyle` built in 02
