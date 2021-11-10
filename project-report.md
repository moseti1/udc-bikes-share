# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Derrick Moseti

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
There were negative datapoints,with which their values had to be changed to zero.


### What was the top ranked model that performed?
WeightedEnsemble_L3 

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
Most of the feature gave more insite on the distribution of data point like `day`, `hour` and `month`

### How much better did your model preform after adding additional features and why do you think that is?
Performance greatly improved the model perfomance. It also lead to improvement in the value of kaggle score.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
Model performance score improved greatly in kaggle score from a value of a `1.39323`  to `0.48303`.

### If you were given more time with this dataset, where do you think you would spend more time?
I would spend alot of time in hyperparameter tuning. Tuning parameters  seem to bring very excellent results.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|initial|time_limit|presets|root_mean_squared_error|1.39323|
|add_features|time_limit|presets|root_mean_squared_error|0.48303|
|hpo|time_limit|presets|root_mean_squared_error|0.47125|



### Create a line plot showing the top model score for the three (or more) training runs during the project.


![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.



![model_test_score.png](img/model_test_score.png)

## Summary
Autoglon is a very excellent tool for doing machine learning tasks fast and for easy setup. Hyperparameter tuning real does the magic here for you to obtain best results.
