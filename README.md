# 📊 Sampling Techniques & Model Performance Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange?style=for-the-badge&logo=scikit-learn)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**A comparative study of sampling techniques on imbalanced credit card data.**


---

## 📝 Overview

This project analyzes the impact of different sampling techniques on the accuracy of various Machine Learning models. Dealing with imbalanced datasets is a common challenge in data science. This repository demonstrates how to:

1.  **Balance** a highly skewed dataset.
2.  **Generate** representative samples using statistical methods.
3.  **Evaluate** model consistency across these samples.

---

## 📂 Dataset

The dataset used is a **Credit Card Fraud Detection** dataset, which is highly imbalanced.
* **Source:** [Creditcard_data.csv](https://github.com/AnjulaMehto/Sampling_Assignment/blob/main/Creditcard_data.csv)
* **Original Distribution:** Class 0 (Legit) vs Class 1 (Fraud) is skewed.
* **Balancing Method:** Random Oversampling (to match majority class).

---

## 🔬 Methodology

### 1. Data Balancing
We balanced the dataset using **Random Oversampling** on the minority class (`Class 1`) until the class distribution was 50-50.

### 2. Sample Size Calculation
We used **Cochran’s Formula** to determine the optimal sample size for a 95% confidence level and 5% margin of error.
> **Calculated Sample Size:** ~385 records

### 3. Sampling Techniques Applied
We compared five different sampling strategies:
* 🟢 **Sampling 1:** Simple Random Sampling
* 🔵 **Sampling 2:** Stratified Sampling
* 🟣 **Sampling 3:** Systematic Sampling
* 🟠 **Sampling 4:** Cluster Sampling
* 🔴 **Sampling 5:** Bootstrap Sampling

### 4. Models Evaluated
* **M1:** Logistic Regression
* **M2:** Decision Tree
* **M3:** Random Forest
* **M4:** Support Vector Machine (SVM)
* **M5:** Gradient Boosting

---

## 📊 Results

The table below shows the accuracy achieved by each model using the training data from different sampling techniques.

| Model | Simple Random | Stratified | Systematic | Cluster | Bootstrap |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Logistic Regression** | 93.46% | 93.79% | 93.46% | 61.44% | 93.46% |
| **Decision Tree** | 98.04% | 99.02% | 99.02% | 61.76% | 97.71% |
| **Random Forest** | 99.35% | **99.67%** | 99.35% | 61.76% | 99.67% |
| **SVM** | 68.63% | 67.97% | 67.65% | 54.25% | 68.95% |
| **Gradient Boosting** | 98.69% | 99.02% | **99.67%** | 61.76% | 98.69% |

> **🏆 Key Insight:** **Stratified Sampling** combined with **Random Forest** or **Gradient Boosting** consistently yielded the highest accuracy.

---

## 👨‍💻 Author

**Devansh Chhabra**  
📧 Email: [devanshchhabr@gmail.com](mailto:devanshchhabr@gmail.com)  

---
