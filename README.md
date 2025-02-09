# AB Test Analysis for E-Commerce Conversion Rates

## Overview

This repository contains a comprehensive analysis of an A/B test conducted on an e-commerce platform. The objective is to understand how different variants affect the session-based conversion rate, how user interactions influence conversion behavior, and how demographic factors play a role. In addition, further analyses—such as clustering, cross-segmentation, and temporal trends—are explored to uncover deeper insights.

## Contents

- **Data Preparation & Cleaning**  
  - Merges `users.csv` and `events.csv`.
  - Handles missing values, duplicates, and converts timestamps.
  - Produces a session-level dataset to accurately compute conversion metrics.

- **Exploratory Data Analysis (EDA)**  
  - Provides summary statistics and visualizations of user events.
  - Includes funnel analysis and a Sankey diagram to visualize user event flows.

- **A/B Test Analysis**  
  - Calculates overall and variant-specific conversion rates.
  - Uses statistical tests (e.g., Chi-Square Test) to assess the significance of differences between variants.
  - Computes 95% confidence intervals and percentage changes between variant conversion rates.

- **Interaction Analysis**  
  - Employs logistic regression to assess the impact of specific events (e.g., `purchase_started`, `share_link`) on the likelihood of conversion.
  - Identifies which user interactions are strong predictors of a purchase.

- **Demographic Analysis**  
  - Examines conversion rates across age groups, countries, and device types.
  - Highlights segments that perform exceptionally well or poorly.

- **Further Analysis**  
  - **Cross-Segmentation Analysis:**  
    Investigates how combinations of user attributes (e.g., age × device) affect conversion behavior.
  - **Clustering Analysis:**  
    Applies unsupervised clustering techniques to identify distinct user segments or archetypes.
  - **Temporal Trends Analysis:**  
    Studies conversion rate patterns over time (daily, weekly, seasonal) to detect trends and anomalies.

## Requirements

- Python 3.13
- Required Python libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scipy
  - statsmodels
  - scikit-learn
  - plotly
  - pytest
  - os

## How to Run

1. **Install Dependencies:**  
   Create a virtual environment and install the required libraries (e.g., using `pip install -r requirements.txt`).

2. **Run the Analysis Notebook:**  
   Open and run the Jupyter Notebook (`main.ipynb`) which contains the complete step-by-step analysis.

3. **Review Outputs:**  
   The notebook produces summary statistics, visualizations, and statistical test results. Review these outputs for actionable insights and recommendations.

## Conclusion

The analysis provides actionable insights into:
- The overall conversion performance (13.55% session-based conversion rate).
- The impact of test variants, with variant_b outperforming variant_a by approximately 19%.
- The influence of key user interactions (e.g., sharing links) on conversion.
- The effect of demographics and device usage on conversion behavior.

Furthermore, the additional mentioned analyses (cross-segmentation, clustering, and temporal trends) could help identify specific user segments, uncover hidden patterns, and detect time-based variations. These insights can guide targeted product optimizations and marketing strategies.

For any additional details or questions, please feel free to reach out.
