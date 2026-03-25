# Inundative sterile parasitoids

R + Quarto project: statistical analyses and manuscript figures for *Modelling the impact of inundative sterile parasitoids and SIT as a novel combination for insect pest eradication* (supporting information).

## Authors

Kiran Jonathan Horrocks<sup>1,2,*</sup>, Adriana Najar-Rodriguez<sup>3</sup>, Rachael Horner<sup>3</sup>, Gonzalo Andres Avila<sup>2,4</sup>, Gregory Ian Holwell<sup>1</sup>, David Maxwell Suckling<sup>1,3,4,+</sup>, Thomas Peter Moore<sup>3</sup>, Lloyd Damien Stringer<sup>3,4</sup>

1. School of Biological Sciences, University of Auckland, Private Bag 92019, Auckland Mail Centre, Auckland, 1142, New Zealand  
2. The New Zealand Institute for Plant and Food Research Limited, Private Bag 92169 Auckland Mail Centre, Auckland, 1025, New Zealand  
3. The New Zealand Institute for Plant and Food Research Limited, Private Bag 4704, Christchurch Mail Centre, Christchurch, 8140, New Zealand  
4. Better Border Biosecurity, Auckland, New Zealand  

\* *Corresponding author* · + *Additional role (see manuscript)*

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
