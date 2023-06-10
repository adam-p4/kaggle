# Microsoft Malware Prediction
This competition was to get the best prediction of which machines are most vulnerable to malware attacks.

My submission is based on the scikit-learn library. It uses random decision forests to learn on the training data and then, given the test data, predicts how likely a machine is to be infected.

First off, I cleaned the datatypes, and truncated the dataframe to reduce computing cost. The data was quite clean from the start, so no further cleaning was necessary.

Then I split the given data into training and validation. I trained the random forest on the training data, and checked how good is the prediction using the validation data. The error function I used for this is the area under the ROC curve of the model from the scikit-learn library.

Finally, I trained the model on both the training and validation sets and fit it to Kaggle's secret validation set, submitting the data to the competition.


Overall, the method I used was very simple and quick, however the accuracy of the predictions suffered as a result. 
Other competitors used a gradient boosting technique instead of a random forest, which is a better fit for this challenge. They also used a weighted feature importance which helped the model learn more accurately. 

While the concepts of gradient boosting are more complex, it was a measurably better performer for the task.
