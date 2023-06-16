# ICR - Identifying Age-Related Conditions
A submission to a [Kaggle competition](https://www.kaggle.com/competitions/icr-identify-age-related-conditions) sponsored by InVitro Cell Research.

Given data with anonymous characteristics, predict whether a patient has at least one of three conditions. The objective is to submit predictions, minimizing a logarithmic loss function.

In this notebook, my objective was to make a thorough study of the data and to find a predictive model that works best.

### Overview of the notebook
#### Dataset Exploration
  * Viewing a sample of the data and the data types
  * Checking for missing and anomalous values
  * Plotting the numerical features 
  * Studying the linear correlation of each feature to the target
#### Data Transformation
  * Cleaning the data by filling missing values and encoding categorical variables
  * Identifying possible ways of feature engineering such as log-transforming and eliminating potentially confusing features
  * Implementing the log-transform and using it on the data
  * Selecting a sampling method to split the data into training and validation sets
#### Model Selection
  * Listing models that are most appropriate to the dataset: Support Vector Machines, Random Forest and Gradient Boosting
  * Making a baseline random forest model 
  * Tuning the random forest
  * Making a Gradient Boosting Machine
  * Making a SVM model 
  * Making a simple Neural Network
  * Comparing all the scores, to select the best model (it was gradient boosting)
#### Improving the Model
  * Using an automatic optimizer to get the best parameters for the model
  * Saving the best performing model
#### Predicting on the test data
  * Transforming the test data in the same manner as the training data
  * Using the best model to predict the target
#### Submitting the results
  * Making a `.csv` file with the required format
