# Early-Stage Diabetes Risk Prediction Using Symptom-Based Machine Learning

## Overview

This project explores how machine learning can be used to predict diabetes at an early stage using simple clinical and symptom-based data. The aim is to provide a low-cost and accessible alternative to traditional diagnostic methods.

## Objectives

* Build a machine learning model for early diabetes prediction
* Handle missing data and class imbalance
* Compare multiple supervised learning algorithms
* Identify important features influencing diabetes risk
* Improve Recall to reduce missed positive cases

## Dataset

The project uses the Pima Indians Diabetes Dataset.

* Total records: 768
* Features: 8 input variables and 1 target variable
* Target: 0 (Non-diabetic), 1 (Diabetic)

Key features include Glucose, BMI, Age, Insulin, Blood Pressure, Pregnancies, Skin Thickness, and Diabetes Pedigree Function.

## Data Preprocessing

* Replaced invalid zero values with missing values
* Applied median imputation
* Removed duplicate records
* Standardized features using scaling


## Exploratory Data Analysis

Different visualizations were used to understand feature relationships and data distribution.

### Correlation Heatmap

<img width="845" height="638" alt="heat" src="https://github.com/user-attachments/assets/a898bb7e-805e-4e8c-b0ab-b3e69b0d088f" />


### Feature Distribution

<img width="975" height="374" alt="image" src="https://github.com/user-attachments/assets/4c1f8175-1018-47b4-a8d7-fd2e73dbba29" />


### Class Distribution

<img width="975" height="770" alt="image" src="https://github.com/user-attachments/assets/68e86596-d38e-4334-8a65-37484b08c552" />


## Models Used

* Random Forest
* Support Vector Machine (SVM)
* Gradient Boosting

## Handling Class Imbalance

The dataset was imbalanced, so random oversampling was applied to improve model performance.

<img width="975" height="603" alt="image" src="https://github.com/user-attachments/assets/8c9b59cd-1718-4844-bf66-7ee69c197a87" />


## Model Optimization

* Hyperparameter tuning using GridSearchCV
* 5-Fold Cross-Validation
* Recall used as the main evaluation metric

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC

## Results

Random Forest performed the best overall.

* Accuracy: 0.7468
* Recall: 0.7222
* F1-Score: 0.6667
* AUC: 0.8104

### Recall Improvement

<img width="860" height="502" alt="image" src="https://github.com/user-attachments/assets/a7eac2ba-96f3-4447-9907-5bb02b5012e6" />


### Confusion Matrix

<img width="975" height="436" alt="image" src="https://github.com/user-attachments/assets/bca08178-a21a-4907-a306-cb5cad8950dc" />


### ROC Curve

<img width="975" height="668" alt="image" src="https://github.com/user-attachments/assets/d8d2c078-5a8d-4043-8975-e5f8a16af012" />


## Key Insights

* Glucose and BMI are the most important features
* Class balancing improves Recall significantly
* Ensemble models perform well on structured data
* High Recall is critical in medical diagnosis

### Feature Importance

<img width="975" height="726" alt="image" src="https://github.com/user-attachments/assets/db308afc-ca7d-4d16-a98b-6535d6f7ae27" />


### Glucose vs BMI

<img width="975" height="646" alt="image" src="https://github.com/user-attachments/assets/219e4c29-585a-4c4c-a16d-5f81fd458ca2" />


## Practical Application

This model can be used in web or mobile applications for early diabetes screening using simple health inputs.

## Limitations

* Dataset limited to a specific population
* No real-world clinical validation
* Limited generalization

## Future Work

* Use real-time datasets
* Improve generalization
* Build a web/mobile application
* Explore advanced models

## Author

*Khadar Basha Shaik
*MSc Data Science
*University of Hertfordshire

## License

This project is for academic and research purposes only.
