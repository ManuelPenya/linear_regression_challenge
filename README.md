# linear_regression
Machine Learning challenge in which, given a dataset, a linear regression predictive model is performed. 

We will make use of `statsmodels` library for model generation due to its great summary information.

Data is divided into train and test accordingly to challenge status.
On training data we perform a linear regression analysis over the 4 features and extract the model and the mean square error. WE can see `feature4` is not really contributing to the model, and hence it might be substracted from the analysis. After this substraction we perform model fitting again and compare both models (with and without `feature4`) with an ANOVA test, verifying both models are feasible.

Finally on test model we perform the predictions, saved in file results.csv