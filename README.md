# US Police Killings Analysis

## Overview
This project analyses police killings in the United States over the past decade using data from [Mapping Police Violence](https://mappingpoliceviolence.us). The dataset has been pre-processed to ensure consistency and facilitate meaningful visualisation and interpretation of trends.

## Data Processing
- **Dataset Cleaning**: Removed incomplete records, reformatted categorical variables, and excluded data from 2024 (as it is not a full calendar year).
- **Filtering and Aggregation**: Data grouped by **year, race, gender, state, and armed status** to derive relevant insights.
- **Racial Population Data**: Integrated census-based racial population statistics to contextualise disparities.

## Key Findings
1. **Overall Trend**: The number of police killings has exhibited an increasing trend over the past decade.
2. **Gender Distribution**: The vast majority of victims are male, with little variation across years.
3. **Age Distribution**: While police killings affect all age groups, there is no significant bias toward older or younger populations.
4. **Racial Disparities**: Black Americans are disproportionately killed by police relative to their population size, in contrast to other racial groups.
5. **State-Level Disparities**: Certain states account for a significantly higher number of killings.
6. **Armed vs. Unarmed Victims**: Despite a considerable portion of victims being unarmed, criminal convictions of police officers remain rare.

## Visualisations
The analysis includes interactive visualisations built with **R Shiny and Plotly** to explore:
- Yearly trends in police killings.
- Breakdown by race, gender, and age.
- Comparison of police killings with state-level racial demographics.
- Proportion of armed vs. unarmed victims.
- Conviction rates of police officers involved in fatal incidents.

## Running the Project
Ensure R and the required libraries are installed before running the script:
```r
install.packages(c("shiny", "plotly", "dplyr", "tidyr", "RColorBrewer"))
```
Run the Shiny app with:
```r
shiny::runApp("us_police_killings_analysis.R")
```

## Conclusion
The analysis highlights systemic disparities in US police killings, particularly concerning racial biases. Future work should focus on integrating more granular data and employing predictive analytics to inform policy discussions and reforms.
