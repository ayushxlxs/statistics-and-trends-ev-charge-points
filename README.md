# Statistics and Trends: EV Charge-Point Availability in England (2022–2024)

## Project Overview

This project analyses electric vehicle (EV) charge-point availability in English dwellings from 2022 to 2024. The analysis explores changes over time and differences between English regions using Python.

## Research Question

**How has the availability of electric vehicle charge points in English dwellings changed across regions from 2022 to 2024?**

## Objectives

- Prepare and clean the supplied dataset.
- Compare charge-point availability across regions and years.
- Visualise trends and regional differences.
- Calculate the four statistical moments: mean, variance, skewness and kurtosis.
- Critically evaluate the findings and limitations of the analysis.

## Dataset

The project uses an ODS spreadsheet containing data for 2022, 2023 and 2024.

- `data/DA8101_Electric_vehicle_charge_points_-_dwellings.ods` — original dataset.
- `data/ev_charge_points_cleaned.csv` — cleaned dataset prepared for analysis.

The cleaned dataset contains regional charge-point availability percentages used in the analysis. The original spreadsheet should be consulted to verify the extracted values and definitions.

**Data source:** Add the official source URL or citation provided with the original dataset here.

## Tools and Libraries

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Google Colab

## Methods

1. Load and inspect the original spreadsheet.
2. Extract and clean the relevant regional data.
3. Check missing values, duplicates and percentage ranges.
4. Create line, bar and box plots.
5. Calculate descriptive statistics and the four statistical moments.
6. Compare regional values across 2022–2024.
7. Interpret the findings and discuss limitations.

## Repository Structure

```text
statistics-and-trends-ev-charge-points/
├── README.md
├── Statistics_and_Trends_EV_Charge_Points_2022_2024.ipynb
├── statistics_and_trends.py
├── data/
│   ├── DA8101_Electric_vehicle_charge_points_-_dwellings.ods
│   └── ev_charge_points_cleaned.csv
└── report.pdf
```

Files such as the Python script and report should be added when they are ready.

## Limitations

This is a descriptive analysis of regional percentages. It does not establish the causes of changes in availability. Results depend on accurate data extraction and consistent definitions across years. Statistical moments calculated from a small number of regions should be interpreted cautiously.

## Reproducibility

The analysis was developed in Google Colab. Upload the original ODS file, install any required dependencies, and run the notebook cells in order to reproduce the analysis.

## Academic Purpose

This repository supports an academic Statistics and Trends assignment. The findings should be interpreted in the context of the supplied data and the limitations described above.
