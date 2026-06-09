# 🏥 Data Preprocessing and Feature Engineering

## 📌 Project Overview

Data preprocessing is one of the most important steps in the Data Science workflow. Raw datasets often contain missing values, inconsistencies, and outliers that can negatively affect machine learning model performance.

This project demonstrates a complete preprocessing pipeline on a healthcare dataset by applying multiple missing value imputation techniques and outlier detection methods. The final cleaned dataset is prepared for predictive analytics and machine learning applications.

---

## 🎯 Objectives

The main objectives of this project are:

- Identify and analyze missing values.
- Apply different missing value imputation techniques.
- Detect and treat outliers.
- Compare multiple preprocessing approaches.
- Generate a clean and machine-learning-ready dataset.
- Improve overall data quality and reliability.

---

## 📝 Problem Statement

A healthcare company has provided patient health records containing missing values and outliers.

The objective is to clean the dataset using multiple imputation and outlier treatment techniques and prepare a reliable dataset for disease risk prediction and other machine learning applications.

---

## 📊 Dataset Description

The dataset contains demographic and medical information of patients.

| Feature | Description |
|----------|-------------|
| patient_id | Unique patient identifier |
| age | Age of patient |
| gender | Male/Female |
| region | Geographic region |
| bmi | Body Mass Index |
| blood_pressure | Blood Pressure Level |
| cholesterol | Cholesterol Level |
| glucose | Blood Glucose Level |
| disease_risk | Target Variable (0 = Low Risk, 1 = High Risk) |

---

## 🔍 Missing Value Imputation Techniques

The following techniques were implemented:

### 1. Simple Imputer
- Mean Imputation
- Most Frequent Imputation

### 2. Missing Indicator
- Created binary indicators for missing observations.

### 3. Random Sample Imputation
- Preserved original data distribution.

### 4. KNN Imputer
- Utilized neighboring observations to estimate missing values.

### 5. MICE (Multiple Imputation by Chained Equations)
- Advanced iterative imputation technique.
- Uses relationships among multiple variables.

---

## 📈 Outlier Detection Techniques

### Z-Score Method
Detects extreme observations using standard deviation.

### IQR Method
Identifies observations outside the interquartile range.

### Percentile Method
Detects extreme values using lower and upper percentile thresholds.

---

## 🛠 Outlier Treatment

### Winsorization

Instead of removing outliers, extreme values were capped using percentile limits to preserve dataset size while reducing the influence of extreme observations.

---

## 🧰 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-Learn
- SciPy
- Jupyter Notebook

---

## 📂 Project Structure


Data_Preprocessing_Project/
│
├── data cleanser.ipynb
├── patient_health_records.csv
├── final_clean_patient_data.csv
├── output.pdf
├── Theory Section.pdf
├── README.md
│
└── Screenshots/
    ├── dataset_head.png
    ├── info.png
    ├── describe.png
    ├── missing_values.png
    ├── simple_imputer.png
    ├── knn_imputer.png
    ├── mice_imputer.png
    ├── zscore.png
    ├── iqr.png
    ├── winsorization.png
    └── final_dataset.png

## 🚀 Project Workflow

1. Dataset Generation
2. Missing Value Introduction
3. Data Exploration
4. Missing Value Analysis
5. Missing Value Imputation
6. Outlier Detection
7. Outlier Treatment
8. Dataset Validation
9. Final Dataset Creation

---

## 📋 Results

The project successfully:

✔ Identified missing values

✔ Applied multiple imputation techniques

✔ Detected outliers using statistical methods

✔ Treated outliers using Winsorization

✔ Generated a clean dataset

✔ Prepared data for machine learning applications

---

## 📉 Key Findings

- MICE produced the most realistic imputations.
- KNN Imputer performed better than simple statistical methods.
- Winsorization effectively reduced outlier influence.
- Data quality improved significantly after preprocessing.

---

## 🎯 Future Scope

- Feature Engineering
- Feature Selection
- Model Building
- Disease Risk Prediction
- Hyperparameter Optimization
- Deployment using Flask/Streamlit

---

## 📚 Conclusion

This project successfully demonstrated the implementation of multiple missing value imputation and outlier treatment techniques in a healthcare dataset.

The final cleaned dataset is accurate, consistent, and ready for machine learning tasks such as disease risk prediction.

---

## 👨‍💻 Author

**Name:** Misari Dhorajiya

**Course:** Data Science with AI & ML

**Academic Year:** 2025–2026

---

⭐ If you found this project useful, consider giving it a star on GitHub.
