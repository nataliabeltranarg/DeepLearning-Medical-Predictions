# Computational Learning and Deep Learning: Intesive Care Unit Prediction Projects 

This repository contains three machine learning projects focused on predicting different outcomes for patients entering the Intensive Care Unit (ICU). The projects use data from MIMIC-III (Medical Information Mart for Intensive Care III) database (publicly available), which includes deidentified health-related data associated with over 25,000 patients who stayed in critical care units at the Beth Israel Deaconess Medical Center between 2001 and 2012. 

## Project Overview 
**1. Mortality Prediction** 
- ***Objective***: Predict the probability of death of patients during an ICU stay.
- ***Dataset***: The dataset includes vital signs and general patient characteristics available on the first day of ICU admissions. 
- ***Methodology***:
    - Handled missing data and created dummy variables for categorical features
    - Applied techniques to address class imbalance
    - *Evaluation metric* used was Area Under the ROC Curve *(AUC)*
- ***Models***:
    - Support Vector Machine (SVM) model to predict patient mortality
    - K-Nearest Neighbors (KNN) model to predict patient mortality

**2. Length of Stay Prediction** 
- ***Objective***: Predict the length of stay (in days) of a patient in the ICU.
- ***Dataset***: The dataset includes vital signs, general patient characteristics, and other relevant features available on the first day of ICU admissions. 
- ***Methodology***:
    - Handled missing data and created dummy variables for categorical features
    - Explored decision tree algorithms and combined them with other models to improve accuracy.
    - *Evaluation metric* used was Root Mean Squared Error *(RMSE)* 
- ***Models***:
    - Neural Networks to forcast patient length of stay 
    - Ensembles to forcast patient length of stay
## Data Sources 

Both projects use data from the MIMIC-III database. Each project's dataset is split into training and test sets, which are used for modeling training, validation, and evaluation. 

- **Training Data**: 'mimic_train.csv'
- **Test Data**:
    - Probability of Death (SVM & KNN): 'mimic_test_death.csv'
    - Length of Stay Prediction: 'mimic_test_los.csv'
      
Additional metadata files:
- **Patient Metadata**: 'mimic_patient_metadata.xlsx'
- **ICD-9 Diagnosis Codes**: 'MIMIC_metadata_diagnose.csv'
- **Co-occurring Diseases**: 'MIMIC_diagnoses.csv' 

## Key Project Sections 
- Exploratory data analysis
- Modeling
- Evaluation


## How to navigate the repository
```bash 
├── 1. Mortality Prediction Project
│   └── ICU_patient_DEATH.ipynb
├── 2. Length of Stay Forecasting Project 
│   └── ICU_patient_LOS.ipynb
├── Data
│   ├── Test
│   │   ├── death of patients
│   │   │    └──  mimic_test_death.csv
│   │   ├── length of stay
│   │   │    └──  mimic_test_los.csv
│   ├── Train
│   │   ├── MIMIC_diagnoses.csv
│   │   ├── MIMIC_metadata_diagnose.csv
│   │   ├── mimic_patient_metadata.xlsx
│   │   └── mimic_train.csv
└── README.md
``` 
