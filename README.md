# Practical 6: Neighbours in space and time

Practical materials for "Data Science for Geographers".

- `Practical_6_Neighbours_in_space_and_time.ipynb` is the practical notebook.
- `datazones.geojson` holds the boundaries of the 1,600 datazones and the council each one is in.
- `datazone_info.csv` gives each datazone's urban/rural classification and SIMD rank.
- `smoking_panel.csv` gives the smoking rate during pregnancy in every datazone in every year from 2012 to 2019 (one row per datazone per year), with the counts it is calculated from.
- `cohort.csv` follows 2,000 women from 2012 to 2019 and records whether each one smokes in every year she took part (one row per woman per year).

The notebook covers defining neighbours (queen, rook and nearest neighbours), spatial weights, spatial and temporal lags, and testing for spatial and temporal autocorrelation. It uses them to evaluate a made-up policy (a cap on tobacco retail licences in two councils from 2016) with difference-in-differences and an event study. The last section uses the cohort to show how attrition can bias a difference-in-differences when the same people are followed over time, and how fixed effects deal with it.

Keep the notebook and the four data files in the same folder.

The data are simulated: every datazone, council, policy and value is fictional.

The notebook needs `tidyverse`, `sf`, `spdep`, `broom`, `modelsummary`, `sandwich` and `fixest`, and an R Jupyter kernel. `sf` may need your operating system's geospatial libraries (GDAL, GEOS and PROJ).
