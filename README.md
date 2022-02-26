# Cardiovascular-Risk-Prediction 
## Problem Statement 
The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients’ information. It includes over 4,000 records and 15 attributes.

Predicting whether a patient has 10-year risk of developing coronary heart disease(CHD) using different Machine Learning techniques on the Framingham dataset.
## Data Description 
#### Demographic: 
* Sex: male or female("M" or "F")
* Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to
whole numbers, the concept of age is continuous)
#### Behavioral 
* is_smoking: whether or not the patient is a current smoker ("YES" or "NO")
* Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be
considered continuous as one can have any number of cigarettes, even half a cigarette.)
#### Medical( history) 
* BP Meds: whether or not the patient was on blood pressure medication (Nominal)
* Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal)
* Prevalent Hyp: whether or not the patient was hypertensive (Nominal)
* Diabetes: whether or not the patient had diabetes (Nominal)
### #Medical(current) 
* Tot Chol: total cholesterol level (Continuous)
* Sys BP: systolic blood pressure (Continuous)
* Dia BP: diastolic blood pressure (Continuous)
* BMI: Body Mass Index (Continuous)
* Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though in fact discrete, yet are considered continuous because of large number of possible values.)
* Glucose: glucose level (Continuous)
#### Predict variable (desired target)
* 10-year risk of coronary heart disease CHD(binary: “1”, means “Yes”, “0” means “No”) -DV
## Model Implementation and Evaluation
Model Name                | Accuracy | Precision | Recall | F1- Score | AUC     |
----------                | ---------|-----------|--------|-----------|---------|
1.Logistic Regression     |      0.76|       0.71|    0.85|       0.78|     0.86|
2.KNN                     |      0.83|       0.85|    0.78|       0.82|     0.91|   
3.SVM                     |      0.79|       0.73|    0.89|       0.80|     0.88|
4.Naive Bayes Classifier  |      0.66|       0.61|    0.85|       0.71|     0.75|
5.Decision Tree Classifier|      0.84|       0.83|    0.83|       0.83|     0.84|
6.Random Forest Classifier|      0.90|       0.88|    0.96|       0.92|     0.97|
7.XGBoost Classifier      |      0.85|       0.78|    0.96|       0.86|     0.92|

* Random Forest Classifier model has given better results as compared to other algorithms.
#### After Hyperparameter Tuning on Random Forest model
* Accuracy is increased from 0.90 to 0.92.
* Precision is increased from 0.87 to 0.88
* Recall is increased from 0.94 to 0.96
* F1-Score is increased from 0.90 to 0.92
