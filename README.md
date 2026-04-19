# Predicting Alzheimer’s Disease Using Machine Learning

## Overview
Alzheimer’s Disease (AD) is a progressive neurodegenerative disorder and a major public health challenge worldwide. Early identification of individuals at risk is critical for improving patient outcomes and enabling timely interventions.

This project develops machine learning models to predict Alzheimer’s Disease diagnosis using clinical, demographic, and behavioral data. By leveraging multiple modeling techniques, the project identifies key predictors and evaluates model performance for early detection and screening.

---

## Background & Significance

- Alzheimer’s Disease affects millions globally and continues to rise with aging populations  
- Early diagnosis is challenging and often relies on cognitive assessments and clinical evaluation  
- Risk factors include age, cardiovascular conditions, depression, and cognitive decline  
- Identifying predictive patterns can support early screening and preventive healthcare strategies  

---

## Dataset & Preprocessing

- **Source:** Kaggle Alzheimer’s clinical dataset  
- **Records:** 2,149 patients  
- **Features:** 34 variables  

### Preprocessing Steps:
- Removed non-informative identifiers (PatientID, DoctorInCharge)  
- Encoded categorical variables  
- Standardized continuous features  
- Created engineered features:
  - BMI categories (normal, overweight, obese)  
  - Comorbidity index  
  - Cognitive impairment flag (based on MMSE)  
- Handled missing values using imputation  
- Performed stratified train-test split (80/20)  

---

## Exploratory Data Analysis (EDA)

- Compared distributions between AD and non-AD groups  
- Identified significant differences in cognitive and functional scores  
- Used:
  - Histograms and box plots  
  - Correlation heatmaps  
  - Group comparisons  

### Key Observations:
- AD patients showed significantly lower MMSE scores  
- Functional ability scores were lower in AD group  
- Behavioral symptoms were more prevalent in diagnosed patients  

---

## Feature Selection & Engineering

### Statistical Methods:
- ANOVA F-test  
- Correlation analysis  

### ML-Based Methods:
- LASSO regression  
- Random Forest feature importance  
- XGBoost feature importance  

### Final Feature Set:
Selected based on:
- Statistical significance  
- Model importance  
- Clinical relevance  

---

## Machine Learning Models

### Algorithms Implemented:
- Logistic Regression  
- Random Forest  
- XGBoost  
- Support Vector Machine (SVM)  

### Handling Imbalance:
- Class weighting / SMOTE  

---

## Model Performance Evaluation

### Metrics Used:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- ROC-AUC  

### Key Results:

- **Random Forest:** ~95.3% accuracy (best overall performance)  
- **XGBoost:** ~94.2% accuracy  
- **Logistic Regression:** ~88.4% (useful for screening)  
- **SVM:** ~84.2% (lower specificity)

---

## Key Insights

- Cognitive measures (MMSE, Functional Assessment) are strongest predictors  
- Behavioral features (memory complaints, confusion) are highly significant  
- Demographic factors have limited impact after controlling for clinical variables  
- Ensemble models outperform linear models due to ability to capture nonlinear patterns  

---

## Limitations

- Cross-sectional dataset (no causal inference)  
- Lack of genetic and biomarker data  
- Potential bias due to imputation  
- Real-world clinical noise  

---

## Tools & Technologies

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- XGBoost  
- Jupyter Notebook  

---

## Key Highlights

- End-to-end machine learning pipeline  
- Feature engineering + selection  
- Multiple model comparison  
- High-performance predictive modeling  
- Healthcare-focused insights  

---


## Author

Tarique Bagalkot
