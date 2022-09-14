# churn_prediction

In this project, I've tried to predict whether the customers will deactivate the service and propose some strategies to avoid that.

The company is Telecom and one of the features of the customers is the Data Plan.

What's interesting is among the customers has a Data Plan, only 10% deactivated the service, so the Data plan can be used as a strategy to retain customers.

The five models were built the predict the customers will deactivate the service:


It was use Random Forest to Feature Selection and only data to train the KNN was scaled.
The data is unbalanced too much, I made testing with oversampling but didn't make difference in the result, actually, without oversampling the algorithms have the best performance.



0 = customer won't desactive || 1 = customer will desactive

Random Forest: accuracy = 92% | precision class 1 = 83% | precision class 0 = 93%

Gradient Boosting: accuracy = 93% | precision class 1 = 88% | precision class 0 = 94%

KNN: accuracy = 89% | precision class 1 = 83% | precision class 0 = 91%

Naive Bayes: accuracy = 83%

Logistic Regression : accuracy = 84%

Gradient Boosting has the best score for precision class 1 with 88%.

