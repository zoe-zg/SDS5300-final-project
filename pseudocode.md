# SDS5300-final-project

Introduction: Brief background on F1 and the goal (predicting race success)

Data cleaning and preparation: 
- load data: from github for portability
- merge data: left join, using driverid, raceid, etc.
- filter for the modern era
- handling missing data, specifically this data set uses "\N" string
- create binary variables for logistic regression for model 2 GLM (e.g. is_podium (finished top 3, Yes/No), is_points (finished top 10, Yes/No)

Data inspection
- some descriptive plots, e.g. speed distribution, pots of finishing positions by team, etc.
- summary stats
- correlation matrix plot, qq-plot, histogram

Correlation and Tests
- correlation between qualifying and race position
- etc
- etc
- bootstrap CI for the correlation
- permutation test to see if a top driver (e.g. max_verstappen) is significantly better than the grid average

Modeling and testing
- model 1 (Linear): predict `positionOrder` (finishing position using multiple regression with backward stepwise selection
- Model 2 (GLM): predict a binary variable (e.g. is_podium, is_points) using binary logistic regression
- model selection and reasoning
- residuals (L.I.N.E)
