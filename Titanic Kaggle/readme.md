# Titanic Kaggle Competition trial

### By: Farahana Suhaimi
### Date: 4/8/2020
### First commit: 4/8/2020

This is the first trial for ML practices. Kaggle page helps me find this first sweet practice.

#### Definition
Problem: Predict the survived people on-board.
Target : To get 90% above accuracy when submitted to the board.
Data : Training set with given survived people and Test set with unknown survival.

#### Resources
There are many resources out there and plenty of notebooks in Kaggle website itself. Main resources for my trial are these:

[Youtube video ](https://www.youtube.com/watch?v=irHhDMbw3xo), [Code 1](https://github.com/justmarkham/scikit-learn-videos/blob/master/10_categorical_features.ipynb), [Code 2](https://github.com/mrdbourke/your-first-kaggle-submission/blob/master/kaggle-titanic-dataset-example-submission-workflow.ipynb), [Code 3](https://github.com/minsuk-heo/kaggle-titanic/blob/master/titanic-solution.ipynb)

#### Trial
I've tried with 5 different machine learning technique using scikit-learn. The best accuracy for now is using GradientBoostingClassifier for features:X_test = test_data.loc[:,['Pclass', 'Sex', 'SibSp', 'Parch', 'Fare']] with 0.77990.