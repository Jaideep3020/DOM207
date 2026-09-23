# Restaurant Transaction Analysis

## Overview
This project analyzes a dataset of restaurant transactions to uncover patterns in tipping behavior and overall bill amounts. By utilizing statistical techniques such as **Analysis of Variance (ANOVA)** and **Welch's independent-samples t-tests**, the analysis identifies actionable insights for restaurant management to optimize revenue and operational efficiency.

## Key Features
*   **Robust Data Cleaning Pipeline:** Handles messy numerical parsing, imputes missing values using statistical modes/medians, and removes duplicates.
*   **Logical Error Handling:** Corrects impossible negative values and flags extreme outliers (using an IQR-fence approach) for sensitivity testing rather than outright deletion.
*   **Statistical Inference:** Employs one-way and two-way ANOVA to understand multi-variable effects, and Welch's t-test to compare distinct groups (e.g., Dinner vs. Lunch, Weekend vs. Weekday).
*   **Actionable Insights:** Automatically translates statistical outputs (F-stats, p-values) into clear, managerial insights that highlight the highest-performing segments and identify areas for targeted interventions.

## Repository Structure
*   **`MP_1.ipynb`**: The main Jupyter Notebook containing the end-to-end data processing and statistical analysis.
*   **`Restaurant.xlsx`**: The original, raw dataset.
*   **`Restaurant_Cleaned.csv`**: The cleansed dataset, ready for visualization and reporting.
*   **`Restaurant_Encoded.csv`**: The dataset with categorical variables encoded, ready for machine learning models.
*   **`analysis.md`**: An automatically generated report summarizing all statistically significant findings and their corresponding managerial insights.
*   **`MP1Specs.pdf`**: The original project specifications and requirements.

## Key Findings Summary
The analysis identified several significant factors driving bill amounts and tips:
*   **Party Size**: Larger parties (>2) contribute significantly higher average amounts per transaction.
*   **Day & Time**: Weekends (specifically Sundays) and Dinner times are the most lucrative segments.
*   **Interactions**: There are notable interactions between variables such as Smoking preference and Gender that jointly shape transaction amounts.

*(For a full breakdown of the statistics and insights, refer to `analysis.md`)*
