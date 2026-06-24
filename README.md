# 🔍 Customer Segmentation & Churn Prediction

![Python](https://img.shields.io/badge/Python-3.8-blue)
![ML](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-green)
![Clustering](https://img.shields.io/badge/Clustering-KMeans-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

> Predicting customer churn and segmenting customers using Machine Learning on a real-world Telecom dataset.

---

## 📋 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [ML Approaches](#ml-approaches)
- [Results](#results)
- [Visualizations](#visualizations)
- [How to Run](#how-to-run)
- [Key Insights](#key-insights)
- [Author](#author)

---

## 📌 Overview
This project solves two real-world business problems for a Telecom company:
- **Churn Prediction** — Predict which customers are likely to leave
- **Customer Segmentation** — Group customers into meaningful segments for targeted retention

---

## 📂 Dataset
| Property | Details |
|----------|---------|
| File | Telco_customer_churn.xlsx |
| Customers | 7,043 |
| Features | 33 |
| Target | Churn Value (1 = Churned, 0 = Retained) |
| Churn Rate | ~26.5% |

**Key Features:** Tenure Months, Monthly Charges, Total Charges, Contract Type, Internet Service, Payment Method, Tech Support

---

## 📊 Project Structure
📦 Customer-Churn-Prediction

┣ 📁 DataSet

┃ ┗ 📄 Telco_customer_churn.xlsx

┣ 📁 EDA & Data Cleaning

┃ ┗ 📄 EDA_and_Cleaning.ipynb

┣ 📁 Machine Learning Implementation

┃ ┗ 📄 Churn_Prediction.ipynb

┣ 📁 Code Segmentation & K-Means

┃ ┗ 📄 Customer_Segmentation.ipynb

┗ 📄 README.md

---

## 🔧 Technologies Used
| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Pandas, NumPy | Data manipulation |
| Matplotlib, Seaborn | Data visualization |
| Scikit-learn | Machine learning models |
| Google Colab | Development environment |

---

## 🤖 ML Approaches
| Approach | Description |
|----------|-------------|
| Baseline Model | Standard Random Forest Classifier |
| Approach 1 | Class Imbalance Handling (class_weight='balanced') |
| Approach 2 | Hyperparameter Tuning (n_estimators, max_depth) |
| Approach 3 | Feature Importance Analysis & Feature Selection |
| Cross Validation | 5-Fold CV for reliable evaluation |

---

## 📈 Results
| Metric | Score |
|--------|-------|
| AUC Score | 0.84 |
| Customer Segments | 3 |

**Segments Identified:**
| Segment | Description |
|---------|-------------|
| 🟢 Budget Loyal | Long term customers, high total charges |
| 🔴 High Risk New | New customers, most likely to churn |
| 🔵 Loyal Premium | High monthly charges, loyal customers |

---

## 📉 Visualizations
| Chart | Insight |
|-------|---------|
| Churn Reason Bar Chart | Support staff attitude is #1 churn reason |
| Feature Importance Plot | Total Charges is the most important feature |
| Correlation Heatmap | Tenure negatively correlates with churn |
| ROC Curve | AUC = 0.84, strong model performance |
| Elbow Method | Optimal K = 3 clusters |
| Segment Scatter Plots | Clear separation between customer groups |

---

## ▶️ How to Run
1. Clone the repository
https://github.com/KunalSingh84/Customer-Segmentation-And-Churn-Prediction
2. Install required libraries
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
3. Upload `Telco_customer_churn.xlsx` to Google Colab
4. Run notebooks in this order:
   - EDA & Data Cleaning
   - Machine Learning Implementation
   - Code Segmentation & K-Means

---

## 💡 Key Insights
- **Total Charges** is the strongest predictor of churn
- **Attitude of support staff** is the #1 reason customers leave
- Customers on **month-to-month contracts** churn the most
- **Fiber optic** users churn more than DSL users
- Customers with **low tenure** are at highest risk

---

## 👤 Author
**Kunal Singh**

[![GitHub](https://img.shields.io/badge/GitHub-KunalSingh84-black?logo=github)](https://github.com/KunalSingh84)
