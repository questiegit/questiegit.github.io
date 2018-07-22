---
layout: post
title: Project 2 at Metis Data Science Bootcamp - Project Luther
---

For the second project at the Metis DataScience Bootcamp, we had to use regression to predict something.  Since most US households have a significant portion of their net worth invested in 
their homes, I wanted to explore this aspect as part of my project.

# THE QUESTIONS: #
With my project I wanted to explore the answer to the following two questions:

1. *Financial:*  Can housing prices be forecast using historical sales data?
2. *Technical:*  Do linear regression models perform better with a larger or smaller number of attributes?

# THE PLAN: #
My plan for the project was the following:
1. Get the zip code from the user for the property whose price I am trying to forecast, and 5 neighboring zip codes.
2. Scrape house sales data from Trulia for these zip codes for the last 9 months
3. Create a regression model to predict pricing based on the various attributes of a house
4. Tune the model to minimize prediction error

# THE RESULTS: Kitchen Sink model

Model Type | Characteristics | Trustworthiness
-----------|-----------------|----------------
The 'Kitchen Sink' model | Factors: 219 | Prediction error (RMSE): $24,362
| | Explanatory Power (R<sup>2</sup>): 90% | Reality Check (Adj. R<sup>2</sup>): -5.4%

Basically the above model can explain 90% of the price variance of the data it is being trained on, and predict housing price with an error of +/- $24,000.  However, due to the large number 
of factors the model is controlling for, it is also picking up a lot of random noise in its correlations.  When this model tries to predict using a previously unseen set of housing 
attributes, its predictions will be significantly off!

Can we improve this model?*

I tried a couple of different regression techniques to see if I could tune the model to make a more realistic prediction.

Model Type | Characteristics | Trustworthiness
-----------|-----------------|----------------
Lasso: | Explanatory Power (R<sup>2</sup): 91% | Prediction error (RMSE): $22,926
| | | Reality Check (Adj. R<sup>2</sup>): -87.7%
Ridge: | Explanatory Power (R<sup>2</sup>): 71% | Prediction Error (RMSE): $41,533
| | | Reality Check (Adj. R<sup>2</sup>): 28%

