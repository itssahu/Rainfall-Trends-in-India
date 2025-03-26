# Rainfall Trends in India Analysis 

## Overview

Rainfall is a critical element of India’s climate system, impacting agriculture, water resources, and the economy. This project performs an in-depth analysis of rainfall trends in India using a comprehensive dataset spanning from 1901 to 2015. We explore long-term trends, seasonal patterns, anomalies, and apply forecasting to predict future rainfall patterns.

## Project Motivation
In this analysis, we aim to uncover long-term trends, seasonal patterns, and anomalies in India’s rainfall data. We will examine historical rainfall trends, detect years with extreme or deficient rainfall, explore relationships between seasonal and annual rainfall, and forecast future rainfall using time series models.

For this analysis, we rely on a dataset containing monthly, seasonal, and annual rainfall measurements spanning over a century. We are using an ideal dataset for this task, which includes monthly rainfall values, seasonal aggregations (e.g., monsoon rainfall), and annual totals, all of which are essential for understanding variability, detecting anomalies, and predicting future trends.
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
   ![raintrend](https://github.com/user-attachments/assets/7afcd6d2-a27f-4140-ae6a-5f8c652d2d3a)
    The above graph shows significant year-to-year variability in India’s annual rainfall, with no apparent long-term upward or downward trend over the century. The red dashed line indicates the mean rainfall, around      which the annual rainfall oscillates. Notable peaks and troughs highlight extreme rainfall events and dry years.![avg_month](https://github.com/user-attachments/assets/5b00b4ec-493b-4f27-80d0-9fead26399df)
    This bar chart illustrates a highly uneven distribution of rainfall across months, with July and August receiving the highest average rainfall. The red dashed line represents the mean monthly rainfall, showing         that most months receive rainfall below the average, except during the monsoon months (June to September).![seasonal_rain](https://github.com/user-attachments/assets/49542d79-dc78-460a-b4cc-ee94ca3b3ffe)
    The seasonal distribution highlights the dominance of the monsoon season (June to September), which contributes the bulk of annual rainfall (around 890 mm). In contrast, the other seasons (January-February, March-     May, and October-December) contribute significantly less to the annual total, which emphasizes the critical role of the monsoon.

2.**Assessing the Impact of Climate Change in the Rainfall Trends in India:**
   ![climate_rain](https://github.com/user-attachments/assets/55738463-58eb-4576-828c-5c36a1d28ebb)
   This graph shows the annual rainfall trends in India (blue line) and a 10-year rolling average (red line) to identify long-term patterns. While annual rainfall exhibits significant variability, the 10-year rolling     average indicates a slight downward trend post-1960, which suggests a possible impact of climate change on rainfall distribution. Periods of higher averages in the early 20th-century contrast with more consistent     but lower averages in recent decades.
   Now, using statistical thresholds (1.5 standard deviations below or above the mean), let’s identify years with extreme or deficient rainfall. This will help detect drought years and periods of excessive rainfall:
   ![image](https://github.com/user-attachments/assets/97298389-6e80-4c43-8052-b10ca405d783)
   The analysis identifies five significant drought years (e.g., 2002 and 2009) and seven extreme rainfall years (e.g., 1917 and 1990) based on deviations from the mean annual rainfall. Seasonal rainfall correlations     with annual totals reveal that the monsoon season (June-September) has the strongest correlation (0.93), which indicates it predominantly drives annual rainfall patterns. In contrast, other seasons like January-       February (0.23) and March-May (0.31) have weaker correlations, which emphasizes the critical role of the monsoon in India’s overall rainfall dynamics.

3. **Anomaly Detection:**  
    Using statistical thresholds and the Isolation Forest algorithm to flag extreme (drought or excessive) rainfall years and months.
   ![anomaly_rain](https://github.com/user-attachments/assets/231d34b6-d5cf-49ad-b5ba-c56aa6ff5416)
   This graph highlights years with significant rainfall anomalies, where annual rainfall deviated substantially from the mean. Drought years (e.g., 1905, 1965, 2002) and extreme rainfall years (e.g., 1917, 1961) are     marked as red points, which showcase outliers in rainfall patterns. While most years cluster around the mean (green dashed line), the anomalies emphasize the variability in India’s rainfall, driven by factors like     monsoonal fluctuations and climate events. This underscores the need for monitoring and preparedness for extreme weather events.
   Now, let’s identify anomalies in monthly rainfall:
   ![monthly_anomaly_rain](https://github.com/user-attachments/assets/e28993ba-274b-4584-9216-8d1d4bd770ff)
   The variability is most pronounced during the monsoon months (June to September), which reflects the critical role of these months in India’s rainfall dynamics. Anomalies in non-monsoon months, while less              frequent,highlight periods of unusual weather patterns, potentially linked to climate variability or regional disturbances. This graph underscores the uneven distribution and high dependence on monsoonal rainfall      for India’s water resources.

5. **Correlating Seasonal Rainfall with Annual Totals:**  
   Examining the correlation between seasonal rainfall and annual totals.
   ![corrain](https://github.com/user-attachments/assets/700dd472-9074-4960-9e06-e1fde4de565b)
   This graph shows the correlation between monsoon rainfall and rainfall during other seasons. The October-December season has the highest correlation (0.29), which suggests a moderate relationship, possibly due to      the post-monsoon retreat rains. The January-February (0.14) and March-May (0.10) seasons exhibit weaker correlations, which indicate minimal dependence on monsoon rainfall. This highlights the dominance of             monsoonal patterns as an independent driver of India’s annual rainfall, with limited spillover effects on other seasons.
  
7. **Grouping Years Based on Rainfall Patterns:**  
     Application of k-means clustering to categorize years as Dry, Normal, or Wet based on rainfall patterns.
    ![clusterrain](https://github.com/user-attachments/assets/dc1f43d0-3f3f-4292-9f1d-bfa2f1618225)
   The clusters reveal that most years fall into the Normal category, while Wet years (above-normal rainfall) are sporadically distributed throughout the timeline, with a concentration in the early and mid-20th           century. Dry years (below-normal rainfall) are more frequent in the latter half of the timeline, which indicates a potential shift in rainfall patterns over time. This clustering emphasizes the variability and         potential long-term changes in India’s rainfall dynamics.

9. **Forecasting Future Rainfall:**  
   Using Prophet Model to forecast annual rainfall for the next 20 years.
   ![prophet](https://github.com/user-attachments/assets/977337e5-b4e0-4972-89ce-d4ae2fb823cb)
   The blue line represents the model’s forecast trend, while the shaded area indicates the confidence interval. The trend reveals a slight decline in annual rainfall over time, with notable year-to-year variability      (black dots representing actual data points). The model captures the variability well but highlights that future rainfall may continue to slightly decrease, which emphasizes the need for adaptive strategies to         manage potential water resource challenges.
## Conclusion
  The analysis of India’s rainfall trends and patterns from 1901 to 2015 reveals significant variability in annual and seasonal rainfall, with the monsoon season (June-September) being the dominant contributor.          Anomalous years of extreme drought and wetness highlight the unpredictability of rainfall, while clustering shows a shift towards more dry years in recent decades. Correlations indicate the limited dependency of       non- monsoon seasons on monsoon rainfall. A time-series forecast using Prophet suggests a slight declining trend in annual rainfall, which emphasises the need for long-term water resource planning and adaptation to    changing climate patterns.
   


