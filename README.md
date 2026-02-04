# Employee Burnout Prediction Analysis 📉

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/4hmed-n/Employee-Burnout-Prediction-AI/blob/main/Employee_Burnout_Prediction_Analysis.ipynb)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Overview
This project leverages machine learning to analyze employee attrition risks and predict burnout levels. By identifying key workplace stressors and segmenting employees into distinct risk profiles, this analysis provides data-driven insights to support HR decision-making and proactive retention strategies.

## 📊 Dataset
* **Source:** Kaggle – [Employee Burnout Analysis](https://www.kaggle.com/datasets/keshabkkumar/employee-burnout-dataset)
* **Description:** A comprehensive dataset containing employee-level metrics including demographics, resource allocation, and self-reported fatigue scores.
* **Target Variable:** `Burn Rate` (0.0 - 1.0)
* **Key Features:** Mental Fatigue Score, Resource Allocation, Designation, Date of Joining.

## ⚙️ Technical Approach
The analysis follows a rigorous data science lifecycle:
1.  **Preprocessing:** Data cleaning, missing value imputation, and temporal feature engineering (deriving `Tenure` from joining dates).
2.  **Exploratory Data Analysis (EDA):** Correlation heatmaps and distribution analysis to identify primary stressors.
3.  **Unsupervised Learning:** K-Means Clustering to discover latent employee risk segments.
4.  **Supervised Learning:** Training a Random Forest Regressor to predict burnout with high precision.
5.  **Interpretability:** Feature importance analysis to quantify the impact of workload vs. tenure.

## 📈 Key Insights & Results
* **Primary Drivers:** **Mental Fatigue Score** is the single strongest predictor of burnout, followed closely by **Resource Allocation** (workload).
* **Tenure Dynamics:** Analysis reveals a non-linear relationship between tenure and burnout, highlighting specific "danger zones" for new hires versus veterans.
* **Segmentation:** Clustering identified **3 distinct employee profiles**, suggesting that generic retention policies are less effective than targeted interventions.
* **Model Performance:** The Random Forest model achieved an **R² > 0.90**, significantly outperforming linear baselines.

## 🚀 Usage (Run in Colab)
You can run the full analysis in your browser without installing anything.

1.  Click the **"Open in Colab"** badge at the top of this README.
2.  **Important:** Since the dataset is hosted in this repository, run the following command in the first cell of the Colab notebook to download the data:

```python
!wget [https://raw.githubusercontent.com/4hmed-n/Employee-Burnout-Prediction-AI/main/employee_burnout_analysis.xlsx](https://raw.githubusercontent.com/4hmed-n/Employee-Burnout-Prediction-AI/main/employee_burnout_analysis.xlsx)
