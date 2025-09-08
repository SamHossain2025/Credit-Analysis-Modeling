<p align="center">
  <img src="3 Assets/Banner.png" width="100%">
</p>

# 🏦 Credit Risk Modeling for Financial Wellness

*A predictive model for assessing default risk and user engagement using real-world fintech data, enhancing strategic credit decisions.*

* Topics covered:**Credit Analytics, Behavioral Modeling, Customer Engagement**
* Models used:**Logistic Regression, Random Forest, XGBoost**
* Skills demonstrated:**Data Cleaning, Feature Engineering, Classification, Imputation**
* Expected outcome:

  * **Predict default & repayment behavior**
  * **Recommend engagement strategies to reduce risk**

---
🔒 Data Privacy Notice

This repository does not include or expose any raw data due to confidentiality agreements. All analysis is based on proprietary financial and behavioral datasets provided by the client.

---

## 👥 Authors

**Sam Hossain** and MMA Team Gordon Members (Alisha Sahota, Anthony Ramelo, Chris Wu, Elizabeth Zhang, Emily Zhao)

---

## 🔍 Problem Statement

**Goal:**

Build a customized credit analysis model to predict repayment and engagement success using psychographic, credit, and behavioral data.

**Challenges Addressed:**

* Proprietary dataset with extensive missing values and feature gaps
* Multi-source integration: loan, behavior, demographics, credit bureau
* Class imbalance between successful and failed repayment cases
* Time-dependent engagement metrics and psychographics

---

## 🔧 Workflow

### ✅ Data Preparation

* Multi-stage imputation: KNN + Iterative (MICE) for missing values
* Winsorization for extreme outliers
* Feature standardization for numeric columns
* Encoding and aggregation of engagement metrics
* Filtering based on valid loan durations and engagement windows

### 🤖 Models Built

| Model   | Type                | Features              | Goal                      | Notes                      |
| ------- | ------------------- | --------------------- | ------------------------- | -------------------------- |
| Model 1 | Logistic Regression | Cleaned + scaled      | Binary (Default vs Repay) | Baseline model             |
| Model 2 | Random Forest       | All features          | Classification            | Captures nonlinear effects |
| Model 3 | XGBoost             | Selected top features | Classification            | Best-performing model      |

**Model Verdict:** XGBoost performed best in balancing recall and precision, crucial for predicting potential write-offs.

<p align="center">
  <img src="3 Assets/Model1.png" width="80%">
  <img src="3 Assets/Model2.png" width="80%">
  <img src="3 Assets/Model3.png" width="80%">
  <img src="3 Assets/Model4.png" width="80%">
</p>

### 💼 Strategic Implementation Flow

* Identify high-risk customers using XGBoost predictions
* Rank user segments based on behavior and credit utilization
* Generate individualized engagement interventions
* Recommend app-based nudges and payment plan restructuring
* Visualize patterns and predictions in interactive dashboards

---

## 🎯 Key Findings

* Engagement frequency (especially quizzes + mood tracking) strongly correlated with financial wellbeing score
* Write-offs often preceded by a drop in engagement >30 days prior to default
* Psychographic variables (e.g., Aptitude for Change) were better predictors than FICO in early signals

---

## 💡 Key Recommendations

* Prioritize app engagement as a leading indicator of financial stress
* Incorporate psychographic variables into loan approval and monitoring
* Build automated risk flags from daily behavioral inputs (e.g., activity decline)

---

## 📊 Output Dashboard

<p align="center">
  <img src="3 Assets/Dashboard1.png" width="80%">
  <img src="3 Assets/Dashboard2.png" width="80%">
  <img src="3 Assets/Dashboard3.png" width="80%">
  <img src="3 Assets/Dashboard4.png" width="80%">
  <img src="3 Assets/Dashboard5.png" width="80%">
</p>

---

## 🚀 How to Run This Project

1. **Clone the repository**

   ```bash
   git clone https://github.com/SamHossain2025/Credit-Analysis-Modeling.git
   cd Credit-Analysis-Modeling
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Jupyter Notebook**

   ```bash
   jupyter notebook
   ```

4. **Open and execute notebooks**

   * `1 Codes/Credit Analysis.ipynb` → Full model pipeline

---

## 🧬 Data Sources

* 📌 Proprietary data from a Canadian financial wellness company (not published for confidentiality)

---

## 🔓 License

This project is licensed under the [MIT License](LICENSE)
