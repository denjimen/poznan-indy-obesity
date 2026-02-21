# Comparing Obesity Rates: Poznań Metropolitan Area vs Indianapolis Metropolitan Area

**Comparative obesity analysis: Poznań Metro (PL612) vs Indianapolis Metro (6-county FIPS). Poznań 20% vs US 38% obesity despite similar metro sizes. Testing if Poznań's 8% bike commuting vs Indianapolis' 0.4% explains the gap using Strava Metro edge counts + CDC PLACES + Eurostat data.**

## Project Overview
Cross-Atlantic health analysis comparing adult obesity trends (2014-2023) between:
- Poznań Metro (city + county, ~1,400 km², NUTS-3: PL612)
- Indianapolis Metro (6-county cluster, ~5,676 km², FIPS: 18097,18057,etc.)

Hypothesis: Poznań's cycling culture (8% bike commute) explains 18-point obesity gap vs US (0.4% bike).

## Data Sources

EU/Poland:
- Eurostat sdg_02_10 (NUTS-3 PL612 obesity rates)
- GUS Local Data Bank (Poznań city/county)
- NFZ health statistics

USA/Indianapolis:
- CDC PLACES 2023 (FIPS county obesity)
- ACS Census (bike commuting)
- Strava Metro (bike edge counts, pending access)

## Analysis Pipeline
1. Data harmonization → 2014-2023 adult obesity % (BMI≥30)
2. Metro aggregation → Poznań city+county vs 6-county IN cluster  
3. Correlation analysis → bike commute % vs obesity rates
4. Plotly dashboard → interactive trends + scatterplots

## Expected Insights
