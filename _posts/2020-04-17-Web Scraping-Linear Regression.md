---
layout: post
title: Movie Revenue Predictor
---

<h2>Proposal</h2>
The movie industry is often thought to be a highly lucrative world. Movie stars, excutives, and other key players make big bucks from the success of films, but at the same time, there is a lot of uncertainty in how a movie does after it is released. This predictive model is a useful tool for those with a large stake in how well a movie does after opening weekend and the financial benefits they reap long-term. 

<h2>Methodology</h2>
First, data from 1000 films was scraped off Box Office Mojo using BeautifulSoup: <a href="https://www.boxofficemojo.com/chart/top_lifetime_gross/?ref_=bo_lnav_hm_shrt">Top Grossing Films</a> 

Raw data can be found <a href="https://github.com/sodas32/Metis-Project-2/blob/master/final_data.csv">here</a>

Code for data cleaning and exploratory analyses can be found <a href="https://github.com/sodas32/Metis-Project-2/blob/master/Project2-WebScraping_EDA.ipynb">here</a>

After sorting through features available from the collected data, the ones  selected for the linear regression model were budget, opening weekend gross, and international gross. The target variable, gross domestic revenue (amount of money made after opening weekend) was feature engineered by subtracting the opening weekend values from the gross domestic values. 

<h2>Initial Analyses</h2>
Three different linear regression models with cross validation were run: simple linear regression, Lasso regularization, and Ridge regularization. Of these three, Lasso regularization resulted in a marginally higher R<sup>2</sup> value and was chosen as the test model. Code for the regression models can be reviewed <a href="https://github.com/sodas32/Metis-Project-2/blob/master/Project%202-Linear%20Regression.ipynb">here</a>

Data was split into training and test sets and model was fit on training data. 
Test data was run in the Lasso model and predicted results graphed against actual values from scraped data. 

![Actual vs Predicted Values]({{sodas32.github.io}}/images/Gross_Rev.png)

<h2>Conclusions</h2>
Three features, budget, opening weekend, and international gross, have some predictive power in determining how much domestic revenue is generated for a film after opening weekend. The linear regression model is accurate for most films but becomes unreliable for outliers. In the future, it would be interesting to group movies by MPAA rating or genre to see whether those factors have an impact on long term revenue generated. 

Review presentation slides <a href="https://github.com/sodas32/Metis-Project-2/blob/master/Metis%20Project%202%20Presentation_Sonali.pdf">here</a>

