# TIRTC_project
Healthcare Analytics: Doctor Visit Patterns & Patient Insights

An exploratory data analysis (EDA) project analyzing patient demographics, health conditions, and insurance coverage to understand key drivers influencing doctor visit frequency.

📌 Project Overview

Understanding patient utilization of healthcare services is crucial for resource planning, insurance modeling, and public health policy. This project processes patient health data to identify patterns between patient demographics, chronic illnesses, insurance types, and doctor visit counts.

Key Objectives

Clean and preprocess raw healthcare records.

Perform Exploratory Data Analysis (EDA) on key numerical and categorical features.

Evaluate the impact of health indicators (illnesses, chronic conditions, reduced activity days) on visit frequency.

Compare healthcare utilization across different insurance and financial support tiers (private, freepoor, freerepat).

Generate actionable data insights and publication-ready visualizations.

📁 Repository Structure

.
├── Healthcare_Analytics.py             # Main analysis Python script
├── 1776250375-P2-Healthcare Analytics...csv # Primary dataset (CSV format)
├── distribution_of_visits.png          # Generated visual chart 1
├── visits_by_gender.png               # Generated visual chart 2
├── illness_vs_visits.png              # Generated visual chart 3
├── healthcare_support_vs_visits.png   # Generated visual chart 4
├── correlation_matrix.png             # Generated visual chart 5
└── README.md                          # Project documentation


📊 Visualizations & Output Insights

The analysis generates five key figures saved to the directory:

distribution_of_visits.png: Frequency plot showing patient visit distributions.

visits_by_gender.png: Bar plot comparing average visit counts between genders.

illness_vs_visits.png: Scatter plot evaluating relationship between illness count, reduced activity days, and doctor visits.

healthcare_support_vs_visits.png: Comparative bar charts across Private Insurance, Low-Income Free Support (freepoor), and Repatriation Support (freerepat).

correlation_matrix.png: Correlation heatmap of all numerical health metrics.

Key Insights Highlighted by the Script

Zero-Visit Baseline: A significant portion of recorded patients made zero visits during the study period.

Chronic Condition Impact: Patients with long-term chronic conditions (lchronic) show higher average visit rates compared to those without.

Financial/Insurance Coverage: Repatriation health assistance recipients (freerepat) show notably higher visit frequencies.

⚙️ Requirements & Installation

Ensure you have Python 3.8+ installed along with the required libraries:

Dependencies

pandas

numpy

matplotlib

seaborn

Install required packages via pip:

pip install pandas numpy matplotlib seaborn


🚀 How to Run

Clone or download this repository.

Ensure your dataset file (1776250375-P2-Healthcare Analytics for Doctor Visits.csv) is placed in the root directory.

Run the script:

python Healthcare_Analytics.py


Note: Fix the syntax issue in line 72 of your Python script before running:

# Change this:
print(f"1. Most patients ({round((df['visits'] == 0).mean() * 100, 2)}%) made 0 visits...")


💡 Potential Future Enhancements

Predictive Modeling: Train Poisson or Negative Binomial regression models to predict visit counts based on health profiles.

Interactive Dashboard: Build a Streamlit or Dash web app to interactively filter patient segments.
