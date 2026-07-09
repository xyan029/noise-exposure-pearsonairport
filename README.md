# Noise Exposure — Toronto Pearson International Airport

Analysis of aircraft noise exposure around Toronto Pearson International
Airport (YYZ). This project combines geospatial and statistical methods (in
**R** and **Python**) to map noise contours, estimate population exposure, and
explore relationships between flight operations and noise levels in the
surrounding communities.

## Project structure

```
noise-exposure-pearsonairport/
├── data/
│   ├── raw/          # Original, immutable source data (git-ignored)
│   └── processed/    # Cleaned / derived datasets (git-ignored)
├── R/                # R scripts (data prep, spatial analysis, plotting)
├── python/           # Python scripts / modules
├── notebooks/        # Jupyter / R Markdown notebooks for exploration
├── output/           # Generated tables, model results (git-ignored)
├── figures/          # Generated maps and plots (git-ignored)
├── .gitignore
├── LICENSE
└── README.md
```

> **Note:** Raw data, processed data, and generated outputs are intentionally
> excluded from version control (see `.gitignore`). Keep a record of data
> sources below so the analysis is reproducible.

## Data sources

<!-- Fill in as you add data -->
- Aircraft noise monitoring data — _source TBD_
- Flight operations / movements — _source TBD_
- Census / population boundaries — _e.g. Statistics Canada_
- Airport boundary & runway geometry — _source TBD_

## Getting started

### R

```r
# Optional: use renv for reproducible package management
install.packages("renv")
renv::init()
```

Common packages for this kind of work: `sf`, `terra`, `tidyverse`, `tmap`.

### Python

```bash
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Common packages: `geopandas`, `rasterio`, `pandas`, `matplotlib`, `contextily`.

## Workflow

1. Place source data in `data/raw/`.
2. Run preparation scripts to write cleaned data to `data/processed/`.
3. Run analysis scripts / notebooks.
4. Generated maps and tables are written to `figures/` and `output/`.

## License

Released under the [MIT License](LICENSE) © 2026 Xiaoyu Yan.
