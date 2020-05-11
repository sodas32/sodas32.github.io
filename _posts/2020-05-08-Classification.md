---
layout: post
title: Diabetic Retinopathy Disease Detection
---

<h2>Background</h2>
Diabetic retinopathy (DR) is a disease that impacts millions of people every year. About one-third of people with diabetes will develop diabetic retinopathy, and the disease can exhibit with a variety of different phenotypes depending on severity. 

There are two forms of diabetic retinopathy, non-proliferative and proliferative. The non-proliferative form is characterized by tiny vessel leaks resulting in macular edema and also ischemia. The disease can progress to its more advanced, proliferative stage, where new vessels start to form, which can then leak into the vitreous humor causing problems in vision. More details about DR can be found <a href="https://www.aao.org/eye-health/diseases/what-is-diabetic-retinopathy">here</a> 

<h2>Objective</h2>
An important part of DR diagnosis is evaluation of fundus images, or pictures of the patient's retina. A physician evaluates and looks for phenotypes that can indicate disease. 

The objective for this project was to develop a machine learning model to classify a patient as having or not having DR based of features from the fundus image. This would automated the diagnosis process and make the evalation less prone to subjectivity based off the thresholds set. 

<h2>Methodology</h2>
The data for this project was acquired from the UCI Machine Learning Repository <a href="http://archive.ics.uci.edu/ml/datasets/Diabetic+Retinopathy+Debrecen+Data+Set"</a>

PostgreSQL on AWS was used to store data for the project. Code for database creation can be found <a href="https://github.com/sodas32/Metis-Project-3/blob/master/Project3_PostgreSQL.ipynb">here</a>

<h2>Initial Analyses</h2>
Numerous classification models were assessed for this dataset, with the target variable being "Class": 1 if the patient has DR, 0 if the patient does not. 
Code for data cleaning and exploratory analyses can be found <a href="https://github.com/sodas32/Metis-Project-3/blob/master/Project3_EDA%26Classification.ipynb">here</a>

<h2>Results</h2>

![Actual vs Predicted Values]({{sodas32.github.io}}/images/Gross_Rev.png)

<h2>Conclusions</h2>
Three features, budget, opening weekend, and international gross, have some predictive power in determining how much domestic revenue is generated for a film after opening weekend. The linear regression model is accurate for most films but becomes unreliable for outliers. In the future, it would be interesting to group movies by MPAA rating or genre to see whether those factors have an impact on long term revenue generated. 

Review presentation slides <a href="https://github.com/sodas32/Metis-Project-2/blob/master/Metis%20Project%202%20Presentation_Sonali.pdf">here</a>
