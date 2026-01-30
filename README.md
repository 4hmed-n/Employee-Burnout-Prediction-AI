# Employee Burnout Prediction Analysis

## 📌 Overview
This project analyzes employee attrition risks to predict burnout levels using machine learning. The analysis focuses on identifying key workplace stressors, segmenting employees into risk profiles using clustering, and building a predictive model to support HR decision-making and retention strategies.

## 📊 Dataset
- **Source:** Kaggle – [Employee Burnout Analysis](https://www.kaggle.com/datasets/keshabkkumar/employee-burnout-dataset)
- **Description:** Employee-level data covering demographics, workload metrics, and fatigue scores.
- **Key Columns:** Mental Fatigue Score, Resource Allocation, Designation, Date of Joining, Burn Rate

## 🔍 Key Analysis Steps
- Data cleaning and missing value handling
- **Feature Engineering:** Creating a `Tenure` variable from joining dates
- Exploratory Data Analysis (EDA) and correlation heatmaps
- **Unsupervised Learning:** K-Means Clustering to identify risk segments
- **Supervised Learning:** Random Forest Regressor for burnout prediction
- Feature Importance analysis to interpret model results

## 📈 Key Insights
- **Mental Fatigue Score** is the single strongest predictor of burnout, followed closely by Resource Allocation (workload).
- Employee **Tenure** shows a non-linear relationship with burnout, indicating different risk levels for new hires vs. veterans.
- Clustering revealed **3 distinct employee profiles**, allowing for targeted interventions rather than generic policies.
- A Random Forest model achieved significantly higher accuracy (**R² > 0.90**) compared to linear baselines.

## 🛠 Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## 📁 Repository Structure
- `employee_burnout_analysis.xlsx` – Dataset used for analysis
- `Employee_Burnout_Prediction_Analysis.ipynb` – Notebook containing the full analysis and modeling
- `README.md` – Project documentation

## ▶️ How to View
The notebook includes all code, outputs, and visualizations and can be viewed directly on GitHub.

To rerun or modify the analysis:
1. Open the notebook in **Google Colab** or on your local machine.
2. Install required libraries if needed:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
