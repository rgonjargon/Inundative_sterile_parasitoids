# Kiran Fruit Flies — Manuscript Analysis

R + Quarto project: statistical analysis and figures for the fruit fly manuscript.

## Folder structure

```text
├── analysis/           # Data and pipeline outputs
│   ├── data/           # Raw spreadsheets (git-ignored)
│   └── output/         # Generated outputs (e.g. models; git-ignored)
├── outputs/            # Manuscript-ready exports
│   └── plots/          # Figures (600 DPI in Quarto YAML)
├── scripts/            # Source reports
│   └── 1_analysis.qmd  # Main analysis (Quarto)
├── .here               # Optional local marker for the here package (git-ignored)
├── .gitignore
└── project.Rproj
```

## Quick start

```bash
cd Kiran_Fruit_Flies
quarto render scripts/1_analysis.qmd
open scripts/1_analysis.html
```

## Prerequisites

- **R** (recent 4.x)
- **Quarto** (`quarto --version` must succeed)
- **R packages** — the document installs missing packages via `ipak()` on render (see the setup chunk in `scripts/1_analysis.qmd`)

## Reproducibility

- Figures use **600 DPI** in the Quarto document YAML (`fig-dpi: 600`).
- Raw data under `analysis/data/` is not tracked by git; obtain data locally or from your team’s archive before rendering.
