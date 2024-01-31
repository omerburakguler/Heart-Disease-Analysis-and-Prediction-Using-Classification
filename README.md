# Heart-Disease-Analysis-and-Prediction-Using-Classification
Project: Heart Disease Analysis and Prediction Using Classification

Author: Ömer Burak Güler

Date: 31/01/2024

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Contents:

1. Objective of the Project
2. Problem Statement
3. Dataset Details
4. Data Preprocessing
5. Exploratory Data Analysis
6. Models Used
7. Results
8. Conclusions

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Objective of the Project:	The primary objective of this project is to develop a predictive model that assesses the risk of heart disease based on our dataset. Aim is to accurately classify individuals into categories representing the likelihood of having heart disease.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Problem Statement: Heart diseases are significant global health concern, and timely identification of individuals at risk is crucial for effective intervention and prevention. The availability of the medical data provides an opportunity to develop a predictive model for heart disease classification. Main problem is to design, develop, and deploy a classification model capable of accurately assessing the likelihood of individuals having heart disease.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Dataset Details:

 a) Dataset Name: heart.csv

 b) Number of Instances: 1319
 
 c) Features:
 
  1)	age: Age of the patient (numerical).
  2) gender: Gender of the patient (0:Female, 1:Male).
  3)	impluse: Impulse of the patient (numerical).
  4)	pressurehight: High blood pressure value of the patient (numerical).
  5)	pressurelow: Low blood pressure value of the patient (numerical).
  6)	glucose: Blood sugar of the patient (numerical)
  7)	kcm: Amount of creatine cinase in blood (numerical)
  8)	troponin: Troponin proteins found in blood value (numerical)

 d) Target Variable:
 
  1) class: Having a heart disease or not, categorical (0:negative, 1:positive)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Data Preprocessing:

 a) Encoding Categorical Variables: Used Label Encoding method for encoding the class values (0: Negative, 1: Positive)

 b) Feature Scaling: Used Standard Scalar for K-Nearest Neighbor models.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Exploratory Data Analysis: Plots are in image folder.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Models Used:

 Model 1: Random Forest Classifier Without Hyperparameter Tuning
 
 Model 2: Random Forest Classifier With Hyperparameter Tuning
 
 Model 3: K-Neighbors Classifier Without Hyperparameter Tuning

 Model 4: K-Neighbors Classifier With Hyperparameter Tuning

 Model 5: Decision Tree Classifier Without Hyperparameter Tuning

 Model 6: Decision Tree Clasifier With Hyperparameter Tuning

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Results:
 <img width="1309" alt="Ekran Resmi 2024-01-31 04 44 58" src="https://github.com/omerburakguler/Heart-Disease-Analysis-and-Prediction-Using-Classification/assets/91601087/982a38d3-cb41-485d-bd7b-d7ef9abe1a29">

 -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Conclusions: After training, testing and evaluating our model we saw that the best results according to our evaluation metrics is given with Model 6. While Random Forest Classifier gives us a 0.979798 accuracy as best, K-Neighbors Classifier gives 0.674242 and Decision Tree Classifier gives 0.982323 accuracy. From these results we can conclude Random Forest Classifier and Decision Tree Classifier fits our dataset well but at the other side K-Neighbor Classifier gives us poor results according to other models. We completed our objective by reaching an accuracy score of 0.982323. We didn’t use StandardScalar on Random Forest Classifier and Decision Tree Classifier because these models don’t need any scaling and when we try to scale them our accuracy drops therefore we didn’t use scaling on them. We add a prediction scenario after creating our models, on our scenario we add a patient that has these features:


age: 30

gender: male

impluse: 85

pressurehight: 150

pressurelow: 90

glucose: 200

kcm: 5

troponin: 0.8

we made prediction on each model with this patient and while model1, model2, model5 and model6 predicted that this patient has heart disease; model3 and model4 predicted that patient did not have any heart diseases. From our evalution results we conclude that model3 and model4 is not reliable and this patient has heart disease.

     
