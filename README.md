# Alzheimer's Disease Prediction using Machine Learning

This project applies machine learning techniques to identify key predictors of Alzheimer’s Disease (AD) and build predictive models for early diagnosis using clinical and demographic data.

---

## Overview

Alzheimer’s Disease is a progressive neurodegenerative disorder that significantly impacts patients and healthcare systems. Early detection is crucial but remains challenging.

This project uses machine learning and statistical analysis to identify the most important features associated with AD diagnosis and to build predictive models for classification.

The analysis is based on a dataset of 2,149 patients with multiple clinical, demographic, and behavioral variables :contentReference[oaicite:0]{index=0}.

---

## Objectives

- Identify key risk factors associated with Alzheimer’s Disease  
- Perform feature engineering and feature selection  
- Build and compare multiple machine learning models  
- Evaluate model performance using classification metrics  
- Provide insights for early detection and screening  

---

## Dataset

- Source: Kaggle (Alzheimer’s clinical dataset)  
- Records: 2,149 patients  
- Features: 34 variables  

### Key Features:
- Demographics: Age, Gender, Education  
- Clinical: Blood pressure, cholesterol, diabetes  
- Cognitive: MMSE score, memory complaints  
- Behavioral: Confusion, disorientation  

---

## Methodology

### 1. Exploratory Data Analysis (EDA)
- Distribution analysis  
- Outlier detection  
- Correlation heatmaps  
- Group comparison (AD vs non-AD)  

---

### 2. Feature Engineering
- BMI categorization (normal, overweight, obese)  
- Comorbidity index creation  
- Cognitive impairment flag (based on MMSE)  
- Encoding categorical variables  
- Feature standardization  

---

### 3. Feature Selection
- ANOVA F-test  
- LASSO regression  
- Random Forest importance  
- XGBoost importance  

A final set of important features was selected based on consensus across methods.

---

### 4. Model Development

Models trained using 80/20 split:

- Logistic Regression  
- Support Vector Machine (SVM)  
- Random Forest  
- XGBoost  

Class imbalance handled using weighting/SMOTE.

---

### 5. Model Evaluation

Metrics used:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- ROC-AUC  

Confusion matrices and ROC curves used for performance analysis.

---

## Results

- **Random Forest** achieved the best performance (~95.3% accuracy)  
- **XGBoost** performed similarly (~94.2%)  
- **Logistic Regression** (~88.4%) useful for screening  
- **SVM** showed lower performance (~84.2%)  

### Key Insights:
- Cognitive features (MMSE, functional assessment) were strongest predictors  
- Behavioral symptoms (memory complaints, confusion) were highly significant  
- Demographic variables had minimal impact  

---

## Limitations

- Cross-sectional dataset (no longitudinal tracking)  
- Missing genetic and biomarker data  
- Potential bias from imputation  
- Real-world noise in clinical data  

---

## Tools & Technologies

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- XGBoost  
- Jupyter Notebook  

---

## Use Case

This project can be used for:

- Early screening of Alzheimer’s Disease  
- Healthcare data science applications  
- Predictive modeling in clinical datasets  
- Research and academic analysis  

---

## Project Files

- Jupyter Notebook with full ML pipeline  
- Project documentation  
- Dataset (if permitted)  

---

## Key Highlights

- End-to-end ML pipeline  
- Feature engineering + selection  
- Multiple model comparison  
- High accuracy predictive model  
- Healthcare-focused analysis  

---

## Author

Tarique Bagalkot
