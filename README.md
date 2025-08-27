Here’s a clean, fully English rewrite of your README while keeping it professional and portfolio-ready:

---

# Understanding Social Behaviors in NYC Parks Under Extreme Heat

This project analyzes how park visitation in New York City changes during **extreme heat events**, using human mobility and weather data. It quantifies the influence of environmental and facility factors — such as tree shade, water proximity, and temporal/spatial patterns—on public space usage, and provides equity- and resilience-focused planning recommendations.

## Background

New York City faces both public health and public space usage challenges during heat waves. This study integrates **park visitation estimates**, **meteorological and heat index data**, and **facility attributes** (shade coverage, water proximity, functional areas) to build a reproducible analysis workflow that informs heat-health interventions and park design strategies.

## Data & Methods

* **Data Sources**:

  * Park visitation data (daily totals redistributed to hourly estimates)
  * Weather and relative humidity (used to calculate and classify Heat Index)
  * Points of Interest (POIs) and park facilities (shade coverage, water proximity, functional categories)

* **Methods**:

  * Data cleaning & feature engineering: redistribute daily visits based on day-of-week patterns to preserve temporal trends; create binary variables for shade/water proximity; generate temporal and spatial dummy variables
  * Statistical modeling: multivariable OLS regression with Variance Inflation Factor (VIF) diagnostics (threshold ≈ 5); stepwise selection using p < 0.05 as a primary reference
  * Visualization: coefficient plots, sub-zone comparisons, and pre/post heat-wave difference analyses

## Repository Structure

```
.
├── README.md
├── src/                 # Reproducible analysis/modeling scripts (main entry: main.py or Makefile)
├── notebooks/           # Exploratory and presentation notebooks
├── reports/             # Papers, posters, slides (poster PDF included)
├── data/
│   ├── raw/             # Raw data (large/sensitive files excluded)
│   └── processed/       # Final analysis datasets
├── .gitignore
```

## Resources

* Poster PDF: [`reports/NYC_Parks_Extreme_Heat_Poster.pdf`](reports/NYC_Parks_Extreme_Heat_Poster.pdf)
* Final Presentation: [`reports/NYC_Parks_Extreme_Heat_Final_Presentation.pdf`](reports/NYC_Parks_Extreme_Heat_Final_Presentation.pdf)
