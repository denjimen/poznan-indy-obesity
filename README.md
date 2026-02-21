# Poznań vs Indianapolis: Obesity & Cycling Analysis

**Comparative study: Why does Poznań have 20% obesity vs Indianapolis' 38%?**

Poznań Metro (PL612, ~1.4M people) vs Indianapolis Metro (6-county, ~2.1M). 
Hypothesis: Poznań's 8% bike commuting explains the gap vs US 0.4%.

## Progress

| Notebook | Status | Description |
|----------|--------|-------------|
| `01_data_collection.ipynb` | Complete | Eurostat PL612 + CDC PLACES APIs connected |
| `02_data_cleaning.ipynb` | Next | Full county aggregation + Polish voivodeships |
| `03_analysis.ipynb` | Planned | Bike commute vs obesity correlations |
| `04_dashboard.ipynb` | Planned | Plotly interactive trends + Strava integration |

## Live Results (Notebook 1)
[View executed notebook](notebooks/01_data_collection.ipynb)
**5 green cells: Eurostat + CDC APIs live**

## Geography
EU/Poland: PL612 (Wielkopolskie) → Poznań city + county
US/Indiana: 6 counties → Marion + 5 surrounding (FIPS: 18097,18057,...)

## Expected Insights
- Poznań: 8% bike commute → 20% obesity (Eurostat)
- Indianapolis: 0.4% bike commute → 38% obesity (CDC)
- Strava Metro: Poznań 10x higher bike edge counts/km²?

## Tech Stack
Eurostat API + CDC PLACES + Plotly + GitHub Actions
Google BigQuery → PostgreSQL → Streamlit dashboard (Q1 2026)

## Next: Notebook 2
Full county datasets + Polish GUS data → obesity heatmaps

---
Built by denjimen | Poznań, Poland → Indianapolis, IN