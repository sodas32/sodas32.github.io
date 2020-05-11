---
layout: post
title: Diabetic Retinopathy Disease Detection
---

<h2>Background</h2>
Diabetic retinopathy (DR) is a disease that impacts millions of people every year. About one-third of people with diabetes will develop diabetic retinopathy, and the disease can exhibit with a variety of different phenotypes depending on severity. 

There are two forms of diabetic retinopathy, non-proliferative and proliferative. The non-proliferative form is characterized by tiny vessel leaks resulting in macular edema and also ischemia. The disease can progress to its more advanced, proliferative stage, where new vessels start to form, which can then leak into the vitreous humor causing problems in vision. More details about DR can be found <a href="https://www.aao.org/eye-health/diseases/what-is-diabetic-retinopathy">here</a> 


![Diabetic Retinopathy]({{sodas32.github.io}}/images/Diabetic-Retinopathy_SS-Graphic-1080x500.jpg)

<h2>Objective</h2>
An important part of DR diagnosis is evaluation of fundus images, or pictures of the patient's retina. A physician evaluates and looks for phenotypes that can indicate disease. 

The objective for this project was to develop a machine learning model to classify a patient as having or not having DR based of features from the fundus image. This would automated the diagnosis process and make the evalation less prone to subjectivity based off the thresholds set. 

<h2>Methodology</h2>
The data for this project was acquired from the <a href="http://archive.ics.uci.edu/ml/datasets/Diabetic+Retinopathy+Debrecen+Data+Set">UCI Machine Learning Repository</a>

PostgreSQL on AWS was used to store data for the project. Code for database creation can be found <a href="https://github.com/sodas32/Metis-Project-3/blob/master/Project3_PostgreSQL.ipynb">here</a>

<h2>Initial Analyses</h2>
Numerous classification models were assessed for this dataset, with the target variable being "Class": 1 if the patient has DR, 0 if the patient does not. 
Code for data cleaning and exploratory analyses can be found <a href="https://github.com/sodas32/Metis-Project-3/blob/master/Project3_EDA%26Classification.ipynb">here</a>

<h2>Results</h2>
The model selection process involved comparing ROC-AUC scores across multiple supervised learning models, with Random Forest classifer yielding the highest value. Accuracy for the chosen model was around 63% and F-score was calculated with beta=1.5. This was done to appropriately weigh recall over precision, since as a physician, falsely predicting DR is preferred over falsely missing a diagnosis. Although more resources will be allocated towards re-testing, the risk of missing a patient with potential disease could be the difference between visual impairment or not. 

Code for the chosen model and metrics can be found <a href="https://github.com/sodas32/Metis-Project-3/blob/master/Project3_Feature%26ModelSelection.ipynb">here</a>

Feature importance graphs showed the relative impact of each feature in the model and how well it correlated with the results. 

![Feature Importance]({{sodas32.github.io}}/images/Feat_imp.png)

<h2>Conclusions</h2>
Presence of microaneurysms and exudates were predictive of diabetic retinopathy and the model was able to categorize a majority of the samples correctly. It is important to note that models like this can improve greatly with larger data sets and adjusting thresholds for categorization can also impact accuracy. In the future, incorporating other measurements such as BMI, blood glucose, or factors like gender and age, could help create an even more comprehensive and predictive model. 

Review presentation slides <a href="https://github.com/sodas32/Metis-Project-3/blob/master/Project_3_Presentation.pdf">here</a>
