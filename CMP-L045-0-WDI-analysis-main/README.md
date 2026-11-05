# CMP-L045-0 Mathematics and Statistics for Data Science — Part 1

Applied problem-solving activity, MSc Data Science, University of Roehampton London.

**Topic:** global income, health and development, analysed with linear algebra, descriptive statistics,
probability models and confidence intervals, using the latest World Bank data.

## Dataset

| | |
|---|---|
| Source | World Bank, World Development Indicators (DataBank) |
| Link | https://databank.worldbank.org/source/world-development-indicators |
| Licence | CC BY-4.0 |
| Downloaded | 2 November 2026 (database last updated 8 October 2026) |
| Coverage | 218 economies × 2015–2025 = 2,398 country-year rows |
| Analysis year | 2024, the latest year in which every indicator is published (health expenditure: latest available, mostly 2023) |
| Variables | GDP per capita (current US$), life expectancy at birth, current health expenditure (% of GDP), urban population (%), internet users (%), fertility rate |

Files in `data/raw/` are exactly as downloaded (`P_Data_Extract_From_World_Development_Indicators.zip`);
`WDI_Data_2015_2025.csv` and `WDI_Series_Metadata.csv` are the two CSVs from that zip, renamed.
`data/wdi_panel_clean.csv` is the cleaned panel written by the notebook.

## Repository contents

```
StudentName.ipynb        all code, with titles (text blocks) and comments (code blocks)
data/raw/                raw World Bank download
data/wdi_panel_clean.csv cleaned country-year panel
figures/                 graphs exported by the notebook (PNG, 200 dpi)
results/                 result tables exported by the notebook (PNG + CSV)
report/                  final report (Word document)
requirements.txt         Python packages
```

## How to run

```bash
pip install -r requirements.txt
jupyter notebook StudentName.ipynb     # then Kernel > Restart & Run All
```

Run from the repository root so the relative paths `data/`, `figures/` and `results/` resolve.

## Notebook outputs used in the report

| Report | File |
|---|---|
| Table 1 | results/tab0_missing.png |
| Table 2 | results/tab1_vectors.png |
| Table 3 | results/tab2a_XtX.png |
| Figure 1 | figures/fig5_correlation_matrix.png |
| Table 4 | results/tab2c_determinant.png |
| Table 5 | results/tab3_descriptives.png |
| Figure 2 | figures/fig1_hist_life_expectancy.png |
| Figure 3 | figures/fig2_hist_gdp_raw_vs_log.png |
| Figure 4 | figures/fig3_scatter_loggdp_life_exp.png |
| Figure 5 | figures/fig4_boxplot_life_exp_by_group.png |
| Figure 6 | figures/fig9_trend_life_expectancy.png |
| Table 6 | results/tab4a_discrete.png |
| Figure 7 | figures/fig6_pmf_discrete.png |
| Table 7 | results/tab4b_continuous.png |
| Figure 8 | figures/fig7_qq_plots.png |
| Table 8 | results/tab5_confidence_intervals.png |
| Figure 9 | figures/fig8_confidence_intervals.png |

## References

World Bank, “World Development Indicators,” DataBank, 2026. Libraries: NumPy, pandas, SciPy, Matplotlib.
The full reference list (IEEE style) is in the report.
