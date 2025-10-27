# 🧠 Customer Segmentation using K-Means Clustering

## 📘 Overview
This project is part of **Modul 9: Clustering** in the Data Science course.  
The objective is to perform **customer segmentation** using the **Mall Customers Dataset** to identify different customer groups based on their demographic and spending behavior.

---

## 📊 Dataset
- **Source:** [Kaggle - Mall Customers Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **Type:** Structured Data  
- **Rows:** 200  
- **Columns:** 5 (`CustomerID`, `Gender`, `Age`, `Annual Income (k$)`, `Spending Score (1–100)`)

The dataset contains demographic and behavioral data of mall customers, which will be used for unsupervised clustering.

---

## 🧹 Data Checking & Preparation
1. Checked for missing values — none found.
2. Encoded categorical variable `Gender` into numeric values.
3. Removed non-influential column `CustomerID`.
4. Standardized numerical features using `StandardScaler` to balance scales across all variables.

---

## 🔍 Exploratory Data Analysis (EDA)
Performed basic data exploration to understand the distribution and relationship between variables:
- Distribution plots for Age, Annual Income, and Spending Score.
- Correlation analysis to examine relationships.
- Identified varying spending behavior among income and age groups.

---

## 🤖 Modelling & Evaluation
- Applied **K-Means Clustering** on standardized data.  
- Determined optimal cluster count using **Elbow Method** and **Silhouette Score**.
- Best model achieved a **Silhouette Score of 0.421** with **10 clusters**.

---

## 📈 Results & Interpretation
Each cluster represents a unique customer group:
- High-income, high-spending customers (loyal, high-value segment).  
- Young, moderate-income, high-spending customers (potential long-term customers).  
- Older, low-spending customers (low-engagement segment).  
- High-income but low-spending customers (selective buyers).

These insights can help mall management tailor marketing strategies based on customer segments.

---

## 🧩 Tech Stack
- Python (Google Colab)
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
