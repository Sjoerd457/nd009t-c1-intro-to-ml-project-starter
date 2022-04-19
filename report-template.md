# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Sjoerd Visser

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
Negative values are not accepted. Therefore the values that are negative are changed into zero's.

### What was the top ranked model that performed?
WeightedEnsemble_L3 was the best model. 

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
The 'datetime' feature was changed into the hour per day as suggested by the exercise. Also the 'weather' and 'season' variables were changed into categorical variables. 

### How much better did your model preform after adding additional features and why do you think that is?
The model improved from 1.79983 to 1.6792. The reason is the model understands the categories and the time of day. 

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
I tried to change a lot of hyper parameters, the only increase came from taking a higher training time. 

### If you were given more time with this dataset, where do you think you would spend more time?
Adding still more training time. 

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|time_limit|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|600|?|?|?|
|add_features|600|?|?|?|
|hpo|?|?|?|?|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](img/model_test_score.png)

## Summary
TODO: Add your explanation
