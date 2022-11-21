# Bank-Churn-Prediction
## Project Overview
In this project, I created a classification model that can determine, depending on specific characteristics of the consumer in question, whether the person is likely to keep their account with a bank open or close it.

Models were built using tree-based methods, starting with a Decision Tree Classifier that was optimized through pruning and ending with a Random Forest Classifier to take advantage of an ensemble of the pruned Decision Trees. The n estimators hyperparameter was then tuned to optimize the Random Forest Classifier.

There were two models made. The first was a baseline model that I could use to calculate baseline metrics without taking into account class imbalance, and the second was a model that used class weights to take into account class imbalance.
The baseline model was found to be inadequate for the project's goal after results analysis revealed that it had an accuracy score of roughly 86.4% and a recall of about 43%. This suggests that the baseline model is not well adapted to accurately detecting the positive cases (churn). The weighted model, on the other hand, was found to be a better fit for the project's goal because I was able to boost recall to 70% while having the same accuracy of about 86.4% by using class weights in it.
