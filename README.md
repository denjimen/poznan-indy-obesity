# Poznań vs Indianapolis: Obesity & Cycling Analysis

**Comparative study: Why does Poznań have 20% obesity vs Indianapolis' 38%?**

Poznań Metro (PL612, ~1.4M people) vs Indianapolis Metro (6-county, ~2.1M). 
Hypothesis: Poznań's 8% bike commuting explains the gap vs US 0.4%.

## Progress

| Notebook | Status | Description |
|----------|--------|-------------|
| [`01_data_collection.ipynb`](notebooks/01_data_collection.ipynb) | ✅ **WorkingProgress** | **Eurostat PL612 BMI data (195 rows)**: Poland obesity 16.7%→18.5% (2014-19), EU rankings, stacked charts |
| `02_data_cleaning.ipynb` | Next | Full county aggregation + Polish voivodeships |
| `03_analysis.ipynb` | Planned | Bike commute vs obesity correlations |
| `04_dashboard.ipynb` | Planned | Plotly interactive trends + Strava integration |

## Live Results (Notebook 1) - **NOW WITH CHARTS**
**Key findings:**
- Poland obesity: **16.7% → 18.5%** (+10% rise, 2014-19)
- EU ranking: Poland mid-pack (Malta 28%+, Italy 13%-)
- **Data:** 13 EU countries × 3 BMI categories × 2 years = 195 rows
- **Chart:** Stacked bars show "normal BMI squeeze"

## Folder Structure
data/ ← eurostat_pl612.csv (live)
output/ ← Charts + CSVs (coming)
dashboard/ ← Streamlit app (Q1 2026)
notebooks/ ← Analysis pipeline

## Geography
**EU/Poland:** PL612 (Wielkopolskie) → Poznań city + county  
**US/Indiana:** 6 counties → Marion + 5 surrounding (FIPS: 18097,18057,...)

## Expected Insights
- Poznań: 8% bike commute → **20% obesity** (Eurostat EHIS)
- Indianapolis: 0.4% bike commute → **38% obesity** (CDC PLACES)
- Strava Metro: Poznań **10x higher** bike edge counts/km²?

## Tech Stack
✅ Eurostat SDMX API + Gzip decompression
✅ Pandas + Matplotlib (live charts)
🔄 CDC PLACES API (next)
🚀 Plotly + GitHub Actions + Streamlit

## Next: More Notebook 1 data collection
- CDC Indianapolis 6-county obesity (PLACES API)
- Polish GUS microdata (voivodeship-level)
- Bike commute ACS data (US Census)
- **Correlation plots** (bike % vs obesity %)

---
**Built by denjimen** | Poznań, Poland → Indianapolis, IN | Feb 2026