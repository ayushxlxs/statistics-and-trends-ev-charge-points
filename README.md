# Statistics and Trends: EV Charge-Point Availability in England (2022–2024)

## Project Overview

This project investigates the availability of electric vehicle (EV) charge points in dwellings across English regions between 2022 and 2024. It uses Python-based data analysis, statistical summaries and visualisations to explore changes over time and differences between regions.

The project was developed as part of a Statistics and Trends academic assignment at the University of Hertfordshire.

## Research Question

**How has the availability of electric vehicle charge points in English dwellings changed across regions from 2022 to 2024?**

## Objectives

- Load, inspect and prepare the original dataset.
- Analyse regional charge-point presence percentages across three years.
- Visualise trends over time and compare regions.
- Calculate the four statistical moments: mean, variance, skewness and kurtosis.
- Compare descriptive statistics across years.
- Evaluate the findings, data quality and limitations of the analysis.

## Dataset Description

The analysis uses the ODS spreadsheet `DA8101_Electric_vehicle_charge_points_-_dwellings.ods`, which contains data for 2022, 2023 and 2024.

The cleaned dataset contains **27 regional observations**, covering nine English regions across three years.

The cleaned CSV contains the following columns:

| Column | Description |
|---|---|
| `year` | Year of observation (2022, 2023 or 2024) |
| `region` | English region |
| `charge_point_presence_pct` | Percentage of dwellings with recorded charge-point presence |

The analysis focuses on the regional percentage measure extracted from the original spreadsheet.

**Data source:** Add the official dataset publisher, source URL and access date here using the details provided with the original dataset.

## Technologies and Libraries

- Python
- pandas — data manipulation and analysis
- NumPy — numerical operations
- Matplotlib — plotting
- Seaborn — statistical visualisation
- SciPy — skewness and kurtosis calculations
- Google Colab — development and execution environment

## Methodology

### 1. Data loading and inspection

The original ODS workbook is loaded into pandas. The yearly sheets are inspected to identify the relevant regional percentage data.

### 2. Data cleaning and preparation

The relevant observations are extracted and organised into a structured DataFrame. The year, region and charge-point presence percentage are retained as analysis variables.

Non-numeric or suppressed entries are converted to missing values rather than being treated as zero. The cleaned dataset is checked for missing values, duplicate rows and valid percentage ranges.

### 3. Exploratory data analysis

Three visualisations are used:

- **Line chart:** compares regional charge-point presence percentages over time.
- **Bar chart:** ranks regions by their recorded percentages in 2024.
- **Box plot with individual observations:** compares the distribution of regional percentages across the three years.

### 4. Statistical analysis

The four statistical moments are calculated:

- **Mean:** average regional percentage.
- **Variance:** dispersion of regional percentages.
- **Skewness:** asymmetry of the distribution.
- **Kurtosis:** tail behaviour relative to a normal distribution, using excess kurtosis.

Yearly summary statistics and regional changes between 2022 and 2024 are also calculated.

### 5. Validation and interpretation

The notebook checks dataset dimensions, year coverage, regional coverage, missing values, duplicate records and percentage ranges. Results are interpreted descriptively, with consideration of data quality and sample size.

## Key Findings

The notebook is designed to identify:

- Changes in average regional charge-point presence between 2022 and 2024.
- Differences in recorded availability between English regions.
- The spread and distribution of regional percentages in each year.
- Regions showing the largest increases or decreases over the period.

Final numerical findings should be reported using the validated outputs from the notebook.

## Limitations

- The analysis is descriptive and does not establish the causes of changes in charge-point availability.
- Regional percentages may conceal differences within individual regions.
- The analysis uses nine regional observations per year; therefore, skewness and kurtosis should be interpreted cautiously.
- Extracted values must be checked against the original spreadsheet headings and definitions.
- Suppressed or unavailable values may limit the observations available for analysis.
- Results depend on consistent definitions and comparable data across the three years.

## Repository Structure

```text
statistics-and-trends-ev-charge-points/
├── README.md
├── Statistics_and_Trends_EV_Charge_Points_2022_2024_.ipynb
├── statistics_and_trends.py
├── data/
│   ├── DA8101_Electric_vehicle_charge_points_-_dwellings.ods
│   └── ev_charge_points_cleaned.csv
└── report.pdf
```

The Python script and report should be added once they have been exported or completed. The original dataset should only be redistributed if its licence and the assignment rules permit it.

## How to Reproduce the Analysis

1. Download or obtain the original ODS dataset from its authorised source.
2. Open the notebook in Google Colab or a compatible Jupyter environment.
3. Upload the original ODS file when prompted.
4. Install the required ODS-reading dependency using `odfpy`.
5. Run the notebook cells in order.
6. Review the data-quality checks, statistical outputs and visualisations.
7. Export the cleaned dataset as `ev_charge_points_cleaned.csv`.

Install the main dependencies locally with:

```bash
pip install pandas numpy matplotlib seaborn scipy odfpy
```

## Conclusion

This project applies descriptive statistics and data visualisation to explore regional EV charge-point presence in English dwellings from 2022 to 2024. Combining temporal comparisons, regional rankings and distributional analysis provides a structured overview of the data.

The findings should be interpreted in light of the dataset's definitions, extraction accuracy and descriptive scope.

## Academic Context

Prepared for the Statistics and Trends assignment at the University of Hertfordshire.

This repository documents the analysis workflow, supporting data files and findings for academic purposes.
