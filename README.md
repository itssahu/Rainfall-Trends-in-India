# Rainfall Trends in India Analysis with Python

## Overview

Rainfall is a critical element of India’s climate system, impacting agriculture, water resources, and the economy. This project performs an in-depth analysis of rainfall trends in India using a comprehensive dataset spanning from 1901 to 2015. We explore long-term trends, seasonal patterns, anomalies, and apply forecasting to predict future rainfall patterns.

## Project Motivation
In this analysis, we aim to uncover long-term trends, seasonal patterns, and anomalies in India’s rainfall data. We will examine historical rainfall trends, detect years with extreme or deficient rainfall, explore relationships between seasonal and annual rainfall, and forecast future rainfall using time series models.

For this analysis, we rely on a dataset containing monthly, seasonal, and annual rainfall measurements spanning over a century. I found an ideal dataset for this task, which includes monthly rainfall values, seasonal aggregations (e.g., monsoon rainfall), and annual totals, all of which are essential for understanding variability, detecting anomalies, and predicting future trends.
Understanding rainfall trends is vital for:
- **Agricultural planning:** Anticipating water availability and crop yield.
- **Disaster management:** Preparing for extreme events such as droughts and floods.
- **Urban water supply:** Planning infrastructure to handle seasonal variability.
- **Climate change adaptation:** Assessing the potential impacts of climate change on rainfall patterns.

## Dataset

The dataset includes:
- **Monthly Rainfall:** Data for each month.
- **Seasonal Aggregations:** Rainfall totals for seasons (e.g., Jan-Feb, Mar-May, Jun-Sep, Oct-Dec).
- **Annual Totals:** Overall yearly rainfall.

## Key Analysis & Insights

1. **Annual Rainfall Trends:**  
   - Plotting annual rainfall with a mean comparison to identify peaks, troughs, and overall variability.
   - *Insight:* Despite year-to-year variability, the 10-year rolling average indicates a slight downward trend post-1960, suggesting climate change impacts.

2. **Monthly & Seasonal Patterns:**  
   - Bar charts reveal that monsoon months (especially July and August) receive the highest rainfall.
   - Seasonal analysis shows the monsoon (June-Sep) contributes the bulk of the annual rainfall, underscoring its critical role.

3. **Anomaly Detection:**  
   - Using statistical thresholds and the Isolation Forest algorithm to flag extreme (drought or excessive) rainfall years and months.
   - *Insight:* Identification of significant drought years (e.g., 2002, 2009) and extreme rainfall years (e.g., 1917, 1990).

4. **Correlation Analysis:**  
   - Examining the correlation between seasonal rainfall and annual totals.
   - *Insight:* The monsoon season shows the strongest correlation with annual rainfall, while non-monsoon seasons have weaker relationships.

5. **Clustering:**  
   - Application of k-means clustering to categorize years as Dry, Normal, or Wet based on rainfall patterns.
   - *Insight:* A noticeable shift toward more dry years in recent decades.

6. **Forecasting Future Rainfall:**  
   - Using Prophet to forecast annual rainfall for the next 20 years.
   - *Insight:* Forecasts suggest a slight declining trend in annual rainfall, emphasizing the need for long-term water resource planning.

## Repository Contents

- **Data:**  
  The `data/` folder contains the raw rainfall dataset.
  
- **Notebooks:**  
  The `notebooks/` folder includes an interactive Jupyter Notebook (`Rainfall_Trends_India_Analysis.ipynb`) that walks through the analysis, complete with visualizations and detailed commentary.

- **Scripts:**  
  The `scripts/` folder has a standalone Python script (`rainfall_analysis.py`) that can reproduce the analysis.

- **Images:**  
  The `images/` folder contains plots generated during the analysis for quick reference and presentation.

- **Forecasts:**  
  Forecast outputs, including the Prophet forecast plot, are stored in the `forecasts/` folder.

## How to Run the Project

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/rainfall-trends-india.git
   cd rainfall-trends-india
