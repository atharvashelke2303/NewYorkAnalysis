# NYC Airbnb Pricing Analysis

Analysis of NYC Airbnb listings to uncover pricing trends across boroughs, room types, and availability using Python, Pandas, Matplotlib and Seaborn.

## Project Overview

This project explores the **New York City Airbnb Open Data (2019)** dataset to identify factors influencing listing prices. Through data cleaning, exploratory data analysis (EDA), feature engineering, and statistical testing, I derived actionable insights for hosts to optimize pricing strategies. The analysis was performed in Google Colab using Python libraries like NumPy, Pandas, Matplotlib, and Seaborn.

### Problem Statement
"What factors influence Airbnb listing prices in New York City, and how can we visualize these trends to help hosts optimize their pricing strategy?"

### Key Features
- **Dataset**: ~48,000 Airbnb listings with 16 attributes (e.g., price, room type, borough, reviews).
- **Techniques**: Data cleaning, outlier detection (IQR), feature engineering (e.g., price per night), ANOVA testing, and geographical visualization.
- **Visualizations**: Histograms, bar plots, boxplots, heatmaps, scatter plots (including a map of NYC).

## Key Findings
- **Borough Impact**: Manhattan listings average ~$180, while the Bronx is lowest at ~$80 (statistically significant via ANOVA).
- **Room Type**: Entire homes/apartments command the highest prices, especially in premium areas.
- **Availability**: High-availability listings (200+ days/year) tend to be cheaper (~$130) than low-availability ones (~$160).
- **Outliers**: ~2,000 listings exceed $334, mostly luxury options in Manhattan.
- **Reviews**: Listings with reviews have slightly higher prices, but location dominates pricing.

## Repository Contents
- **`NYC_Airbnb_Analysis.ipynb`**: Jupyter Notebook with all code, comments, and visualizations.
- **`AB_NYC_2019.csv`**: Original dataset (sourced from [Kaggle](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)).
- **`cleaned_airbnb_nyc.csv`** (optional): Cleaned dataset generated during analysis.
