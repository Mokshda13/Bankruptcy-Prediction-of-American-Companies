
**Bankruptcy Prediction of American Companies**

This project aims to predict the likelihood of bankruptcy for American companies using historical financial data. The goal is to identify companies at risk by analyzing key financial indicators and applying machine learning techniques to enable better decision-making for investors, lenders, and policymakers.

---

**Project Objectives**

* Predict bankruptcy using financial metrics
* Identify the most influential financial indicators
* Segment companies into financial risk groups
* Automate the machine learning pipeline using Apache Spark and MLflow

---

**Business Questions**

* What financial patterns separate bankrupt and non-bankrupt companies
* Which metrics are most predictive of bankruptcy risk
* Can companies be grouped by financial health
* How have bankruptcy rates changed over time

---

**Dataset Summary**

* Data Source: Financial statements from American companies (1999 to 2018)
* Size: Approximately 10000 records and 64 features
* Target Variable: Bankruptcy class (1 for bankrupt, 0 for non-bankrupt)
* Important Features: Net income, retained earnings, total liabilities, EBITDA, interest coverage ratio

---

**Technology Stack**

* Languages: Python, SQL
* Tools: Apache Spark, Databricks, MLflow
* Libraries: Scikit-learn, Pandas, Matplotlib, Seaborn
* Storage: Parquet
* Models: Logistic Regression, Gradient Boosting, K-Means Clustering
* MLOps: Spark ML Pipelines, CrossValidator, MLflow for model tracking

---

**Exploratory Data Analysis**

* Created new features like debt to equity ratio and interest coverage ratio
* Analyzed revenue, profitability, and asset patterns
* Observed that bankrupt firms generally have lower EBITDA and net income
* Attempted SMOTE for class balancing but reverted to original data due to performance drop

---

**Modeling Approach**

Logistic Regression

* Accuracy: 93.3 percent
* AUC: 65.0 percent
* Suitable for interpretability but limited in capturing complexity

Gradient Boosting

* Accuracy: 93.3 percent
* AUC: 72.8 percent
* Better at capturing non-linear relationships

---

**Clustering Analysis**

* Used Principal Component Analysis to reduce dimensionality
* Applied K-Means clustering with three clusters
* Grouped companies into low risk, medium risk, and high risk categories

---

**MLOps Integration**

* Automated feature transformations and model training using Spark Pipelines
* Used MLflow to track experiments and log hyperparameters
* Registered best-performing models for deployment

---

**Key Insights**

* Net income, EBITDA, and retained earnings are strong bankruptcy predictors
* Debt alone is not always a risk factor without considering profitability
* Clustering helps identify risk segments for more informed decisions
* Real-time monitoring and advanced models can improve future predictions

---

**Future Improvements**

* Collect more bankruptcy examples to improve class balance
* Explore advanced models like XGBoost and neural networks
* Integrate real-time financial data for live prediction

---
