# Surge_Price_Prediction
# Problem
The problem was to predict the surge pricing type of a cab aggregator. This is a classic classification problem which is very important as the cab aggregators are expanding aggressively. This would solve their dilemma of supply-demand based pricing which essentially solve in matching right cabs with the right customers.

This type of problem requires a lot of customer data as well as trip related data. Due to data limitation, it is essential to perform feature engineering. In this problem, there were 3 continuous variables which were aggregated based on other discrete variables. New features such as mean, median, min and max for these continuous variables based on other discrete features were derived. This has led to a little bit increase in accuracy but not to greater extent.

Different algorithms were used to build the model especially I tried with various machien learning algorithm. Ensemble of the best performing models were tried to see the accuracy score on the test data set. however, individual model LGBM performed better on test data set. 

# Pre-processing ideas

The pre-processing steps mainly include missing value imputation and feature engineering

Missing values were imputed with mean/median and mode for continuous and discrete features respectively
Continuous features (var1, var2, var3) were aggregated using discrete variables and new features such as mean, median, minimum, maximum values per category were obtained.

# Final model

Final model was selected based on accuracy score of each model as well as model ensembles. It was observed that  LGBM performed better than other models.
