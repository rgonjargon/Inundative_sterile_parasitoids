# Inundative sterile parasitoids

R + Quarto project: statistical analyses and manuscript figures for *Modelling the impact of inundative sterile parasitoids and SIT as a novel combination for insect pest eradication* (supporting information).

## Folder structure

```text
├── analysis/           # Data and pipeline outputs
│   └── data/           # Raw spreadsheets (git-ignored)
├── outputs/            # Manuscript-ready exports
│   └── plots/          # Figures (600 DPI in Quarto YAML)
├── scripts/            # Source reports
│   └── 1_analysis.qmd  # Main analysis (Quarto)
├── .gitignore
└── project.Rproj
```

## Quick start

```bash
cd Inundative_sterile_parasitoids
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
