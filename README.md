## US Traffic Accident Analysis and Recommendations

## Overview

This project analyzes U.S. traffic accident data to identify key factors that contribute to accident severity and frequency. The goal is to uncover high-risk conditions related to weather, time, location, and road features, and to provide data-driven recommendations that can help transportation officials improve road safety.

## Dataset

The raw and cleaned datasets are not included due to GitHb file size limits. The analysis notebook documents contain all data cleaning steps.

1. Source: U.S. Accidents Dataset (https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents)
2. Size: ~7.7 million accident records  
3. Key Attributes:  
  - Location (State, City, Latitude, Longitude)  
  - Time (Start Time, Hour)  
  - Weather (Visibility, Temperature, Wind Speed, Weather Condition)  
  - Road Features (Junction, Bump, Railway, Roundabout, Traffic Signal)  
  - Severity (1–4)

## Tools and Technologies

1. Python: Pandas, NumPy, Matplotlib, Seaborn  
2. Statistical Methods: Correlation analysis, Chi-square tests, Kruskal–Wallis test  
3. Visualization: Tableau  
4. Environment: Jupyter Notebook

## Data Preparation

1. Removed missing and invalid records
2. Converted time fields to extract hour, month and year
3. Addressed skewed numerical variables using transformations and selective IQR capping
4. Excluded severity from inappropriate transformations
5. Saved a cleaned dataset for visualization in Tableau

## Exploratory and Statistical Analysis

1. Analyzed accident patterns by hour, weekday, state, and weather
2. Used correlation analysis to assess relationships between severity and weather variables
3. Applied non-parametric tests (Kruskal–Wallis) where assumptions for parametric tests were violated
4. Evaluated the impact of road features on average accident severity

## Key Findings

1. Poor weather conditions and low visibility are linked to higher accident severity
2. Accidents peak during rush hours and nighttime
3. Road features such as junctions, railways, and roundabouts show higher average severity
4. High-traffic states account for a disproportionate number of severe accidents

## Dashboards

### Dashboard 1: Executive Summary

    - Total Accidents
    - Accident Hotspot Map
    - Accidents by Hour of Day
    - Severity by Weather Condition

### Dashboard 2: Deep Dive Analysis
    - Severity vs Temperature
    - Severity vs Visibility
    - Road Features Impact
    - Severe Accident Rate by State

# Recommendations

1. Improve visibility measures during poor weather (better lighting, alerts, signage)
2. Enhance traffic control and safety measures at high-risk road features
3. Deploy targeted enforcement and awareness campaigns during peak accident hours

# Limitations

1. Correlation does not imply causation
2. Reporting inconsistencies across states
3. Some weather variables contain missing or extreme values
4. Severity is an ordinal variable treated numerically for analysis

# Next Steps

1. Incorporate traffic volume data for stronger causal insights
2. Apply predictive modeling to forecast high-risk scenarios
3. Integrate real-time weather and traffic feeds
4. Conduct before-and-after studies to measure intervention impact


