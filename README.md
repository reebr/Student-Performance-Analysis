# Student-Performance-Analysis
# Student Performance Analysis Using Linear Regression

## 📌 Project Overview
This project analyzes the factors influencing students’ final exam performance using statistical methods and multiple linear regression modeling. The analysis includes data preprocessing, descriptive statistics, correlation analysis, visualization, outlier detection, model building, and evaluation.

The goal is to identify which academic and behavioral attributes best predict the final exam score (*Exam_Score*) and to evaluate how accurately these variables can be used for prediction.

---

## 📊 Dataset Description
- **Number of Records:** 6,607  
- **Number of Features:** 20  
- **File Format:** CSV  
- **Target Variable:** `Exam_Score`

### Key Features Used in the Model:
- `Attendance`  
- `Hours_Studied`  
- `Previous_Scores`  
- `Tutoring_Sessions`  
- `Access_to_Resources` (encoded into dummy variables)

---

## 🔧 Methods and Techniques
The project includes the following steps:

### 1. Data Preparation
- Removal of missing values  
- One-hot encoding for categorical variables  
- Dataset cleaning and feature extraction  

### 2. Descriptive Analysis
- Summary statistics for all selected variables  
- Distribution inspection using histograms  

### 3. Correlation Analysis
- Pearson correlation with the target variable  
- Identification of the strongest predictors  

### 4. Outlier Detection
- Boxplots  
- IQR (Interquartile Range) method  
- Decision to retain outliers as valid observations  

### 5. Visualizations
- Histograms  
- Scatter plots with regression lines  
- Bar charts for resource access levels  
- Residual and QQ-plots for diagnostics  

### 6. Predictive Modeling
A multiple linear regression model was built using the selected predictors.

### 7. Model Evaluation
- **R²**: 0.6824  
- **RMSE**: 2.08  
- **MAE**: 1.12  
- Residual diagnostics to verify model assumptions  

---

## 🧠 Key Findings
- **Attendance**, **hours studied**, and **tutoring sessions** were the strongest positive predictors of exam performance.  
- Limited access to educational resources significantly decreased exam scores.  
- The regression model performed well and explained approximately **68%** of the variance in exam scores.  
- Outliers were valid and retained, and residual diagnostics confirmed model reliability.

---

## 📁 Repository Contents
- `StudentPerformanceFactors.csv` — Dataset  
- `analysis_code.ipynb` — Full Python code  
- `Final_Report.pdf` — Project report  
- `README.md` — Project documentation (this file)

---

## ▶️ How to Run the Code
1. Install required Python libraries:
   ```bash
   pip install pandas numpy matplotlib scikit-learn scipy
