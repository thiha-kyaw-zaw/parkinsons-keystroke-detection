# 🧬 Parkinson’s Disease Detection using Keystroke Dynamics

## 📌 Overview

This project explores the use of **keystroke dynamics** (typing patterns) combined with **machine learning** to detect early-stage Parkinson’s Disease (PD).

Traditional diagnostic methods are often subjective and may lead to delayed or incorrect diagnosis. This project proposes a **non-invasive, data-driven approach** for early detection.

---

## 🎯 Objective

* Identify early signs of Parkinson’s Disease using typing behaviour
* Apply feature selection to improve model performance
* Compare machine learning models for accurate classification

---

## 📊 Dataset

* Source: PhysioNet (Tappy Keystroke Dataset)
* Includes:

  * Hold time
  * Flight time
  * Latency time
  * Demographic and clinical data

---

## ⚙️ Methodology

### 1. Data Preprocessing

* Merged keystroke and user datasets
* Removed duplicates and missing values
* Outlier removal using IQR
* Feature scaling (Min-Max scaling)

### 2. Feature Engineering

* Created age and age groups
* One-hot encoding for categorical variables
* Removed irrelevant features

### 3. Feature Selection

* Recursive Feature Elimination (RFE)
* Identified most important keystroke features

### 4. Handling Imbalance

* Applied SMOTE (Synthetic Minority Over-sampling Technique)

### 5. Machine Learning Models

* Random Forest
* Logistic Regression

---

## 📈 Results

| Model               | Accuracy |
| ------------------- | -------- |
| Random Forest       | 96.46%   |
| Logistic Regression | 94.96%   |

* Feature selection + SMOTE significantly improved performance
* Random Forest achieved the best results

---

## 🛠️ Tech Stack

* Python
* Scikit-learn
* Pandas, NumPy
* Matplotlib, Seaborn

---

## 🚀 Future Improvements

* Use larger and more diverse datasets
* Apply deep learning models
* Explore real-time detection systems

---

## 📌 Author

Thiha Kyaw Zaw
MSc Data Science, University of Sheffield

### Confusion Matrix
![Confusion Matrix](results/user_reduction_bar_chart.png)
