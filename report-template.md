# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Derrick Moseti

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: Predictions dataframe needed to be turned into a `csv` file using `.to_csv` method of python.

### What was the top ranked model that performed?
TODO: The top Ranked model was WeightedEnsemble. I had the highest score of all. 

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: Add your explanation

### How much better did your model preform after adding additional features and why do you think that is?
TODO: The model score of Weighted Ensemble increased

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: The model score in creased when i introduced the `num_trials` hyperparameter. 

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: Add your explanation
I would spend time in doing proper feature selection. The models seemed to respond better with more feature. Also time on parameter tuning would be excellent. 

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|WeightedEnsemble|default|default|search_strategy, num_trials,scheduler|1.37974|
|initial|default|default|default|1.37132|
|add_features|default|default|default|1.37526|
|hpo|search_strategy|scheduler|num_trials|1.37974|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: Of all the model, WeightedEnsemble seemed to work best.Its rmse was 
