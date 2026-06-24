# Customer Segmentation & Churn Prediction

![Python](https://img.shields.io/badge/Python-3.8-blue)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![ML](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-green)
![Clustering](https://img.shields.io/badge/Clustering-KMeans-orange)
![Colab](https://img.shields.io/badge/Google-Colab-yellow)

This is my machine learning project where I worked on predicting customer churn and grouping customers into segments using a real Telecom dataset.

---

## Table of Contents
- [About the Project](#about-the-project)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Tools & Libraries](#tools--libraries)
- [What I Did](#what-i-did)
- [Approaches](#approaches)
- [Results](#results)
- [How to Run](#how-to-run)
- [What I Achieved](#what-i-achieved)
- [What I Learned](#what-i-learned)

---

## About the Project
I built this project to understand how telecom companies can predict which customers are going to leave and why. The project has two main parts:
- Predicting churn using Random Forest
- Grouping customers into segments using KMeans Clustering

---

## Dataset
- File: Telco_customer_churn.xlsx
- 7,043 customers and 33 columns
- Target column: Churn Value (1 = left, 0 = stayed)
- About 26.5% of customers churned

---

## Project Structure
📦 Customer-Churn-Prediction

┣ 📁 DataSet

┃ ┗ Telco_customer_churn.xlsx

┣ 📁 EDA & Data Cleaning

┃ ┗ EDA_and_Cleaning.ipynb

┣ 📁 Machine Learning Implementation

┃ ┗ Churn_Prediction.ipynb

┣ 📁 Code Segmentation & K-Means

┃ ┗ Customer_Segmentation.ipynb

┗ README.md

---

## Tools & Libraries
- Python
- Pandas and NumPy for data handling
- Matplotlib and Seaborn for graphs
- Scikit-learn for machine learning
- Google Colab for coding

---

## What I Did
1. Loaded and explored the dataset to understand patterns
2. Cleaned the data and removed unnecessary columns
3. Visualized churn reasons, monthly charges, tenure and more
4. Trained a Random Forest model to predict churn
5. Handled class imbalance and tuned the model
6. Used KMeans to group customers into 3 segments
7. Evaluated model using AUC Score and ROC Curve

---

## Approaches

**Baseline Model**
Started with a standard Random Forest Classifier with 100 trees to get an initial accuracy and understand the data.

**Approach 1 — Handling Class Imbalance**
The dataset had more retained customers than churned ones. Used class_weight='balanced' to make the model pay more attention to churned customers and improve recall.

**Approach 2 — Hyperparameter Tuning**
Tried different combinations of number of trees (100 to 500) and max depth (5 to 20) to find the best performing model. Sorted results by recall to find the best churn detector.

**Approach 3 — Feature Importance & Selection**
After training, extracted feature importance scores from the model. Identified and removed the least important features to create a leaner and cleaner model.

**Cross Validation**
Used 5-Fold Cross Validation to get a more reliable accuracy and recall score across different splits of the data.

---

## Results
- AUC Score: 0.84
- 3 customer segments found:
  - Budget Loyal Customers — stay long, pay less monthly
  - High Risk New Customers — new customers likely to leave
  - Loyal Premium Customers — high monthly charges, loyal

---

## How to Run
1. Download or clone this repository : https://github.com/KunalSingh84/Customer-Segmentation-And-Churn-Prediction
2. Install the libraries: 
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
3. Upload the dataset to Google Colab
4. Run the notebooks one by one in order

---

## What I Achieved
- Built a churn prediction model with an AUC score of 0.84
- Successfully identified 3 distinct customer segments using KMeans
- Found that Total Charges is the strongest predictor of churn
- Discovered that attitude of support staff is the #1 reason customers leave
- Created visualizations like Feature Importance Plot, ROC Curve, Correlation Heatmap and Churn Reason Chart that give real business insights
- Organized the entire project into a clean folder structure on GitHub

---

## What I Learned
- How to handle real world messy data
- Why class imbalance matters in ML
- How KMeans clustering works in practice
- How to evaluate a model properly using AUC and ROC
- How feature importance helps explain model predictions

---

## Author
Kunal Singh 
