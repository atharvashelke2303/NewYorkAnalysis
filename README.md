# NYC Airbnb Pricing Analysis

Analysis of NYC Airbnb listings to uncover pricing trends across boroughs, room types, and availability using Python, Pandas, and Seaborn.

## Project Overview

This project explores the **New York City Airbnb Open Data (2019)** dataset to identify factors influencing listing prices. Through data cleaning, exploratory data analysis (EDA), feature engineering, and statistical testing, I derived actionable insights for hosts to optimize pricing strategies. The analysis was performed in Google Colab using Python libraries like NumPy, Pandas, Matplotlib, and Seaborn.

### Problem Statement
"What factors influence Airbnb listing prices in New York City, and how can we visualize these trends to help hosts optimize their pricing strategy?"

### Key Features
- **Dataset**: ~48,000 Airbnb listings with 16 attributes (e.g., price, room type, borough, reviews).
- **Techniques**: Data cleaning, outlier detection (IQR), feature engineering (e.g., price per night), ANOVA testing, and geographical visualization.
- **Visualizations**: Histograms, bar plots, boxplots, heatmaps, scatter plots (including a map of NYC).

## Key Findings & Conclusions

After a comprehensive analysis, here are the insights and implications:

- **Price Distribution and Boroughs**:
  - Prices vary significantly across boroughs (ANOVA, p < 0.05). Manhattan has the highest average price (~180 USD), while the Bronx is the lowest (~80 USD), reflecting location-driven demand and cost of living differences.
  - Entire homes/apartments command higher prices than private or shared rooms, especially in Manhattan and Brooklyn.

- **Room Type Impact**:
  - Room type strongly influences price, with entire homes/apartments averaging over $200 in premium boroughs, while shared rooms stay below $70. Hosts can optimize pricing by offering larger spaces in high-demand areas.

- **Geographical Patterns**:
  - Higher-priced listings cluster in Manhattan and parts of Brooklyn, aligning with urban density and tourist hotspots. Lower prices dominate in outer boroughs like Queens and the Bronx.

- **Outliers**:
  - ~2,000 listings exceed ~$334 (IQR method), mostly in Manhattan, indicating luxury or premium offerings that skew the distribution.

- **Availability Trends**:
  - Listings with higher availability (200+ days/year) have lower average prices (~$130) compared to low-availability listings (~$160). This suggests high-availability listings may be less desirable or priced lower to attract bookings.
  - Entire homes with low availability fetch higher prices, hinting at exclusivity.

- **Review Activity**:
  - Listings with reviews have a slightly higher median price (~$130) than those without (~$110), suggesting reviewed properties may be more established. However, location and room type dominate pricing over reviews.

- **Feature Insights**:
  - The `price_per_night_stay` feature shows longer minimum stays reduce nightly costs, appealing to budget travelers. Weak correlations between price and reviews/availability reinforce location’s dominance.

- **Business Implications**:
  - **For Hosts**: In Manhattan and Brooklyn, charge premium rates for entire homes but monitor availability to avoid seeming undesirable. In outer boroughs, target budget travelers with competitive pricing and flexible stays. Encourage reviews to signal quality, though it’s not a major pricing lever.
  - **Strategic Takeaway**: Location and room type are the primary pricing drivers, with availability and reviews as secondary factors.

## Repository Contents
- **`NYC_Airbnb_Analysis.ipynb`**: Jupyter Notebook with all code, comments, and visualizations.
- **`AB_NYC_2019.csv`**: Original dataset (sourced from [Kaggle](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)).
- **`cleaned_airbnb_nyc.csv`** (optional): Cleaned dataset generated during analysis.
