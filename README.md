# Metrics_to_Evaluate
Machine Learning - Classification Metrics, Regression Metrics


## Classification Metrics:
# How to use the following metrics:

1. Classification Accuracy.
2. Log Loss.
3. Area Under ROC Curve.
4. Confusion Matrix.
5. Classification Report.

## 1. Classification Accuracy
* Classification accuracy is the number of correct predictions made as a ratio of all predictions made.

* This is the most common evaluation metric for classification problems, it is also the most misused. It is really only suitable when there are an equal number of observations in each class (which is rarely the case) and that all predictions and prediction errors are equally important, which is often not the case.
*This can be converted into a percentage by multiplying the value by 100. (0.778)*100 -> 77.8

## 2. Log Loss
* Logistic loss (or log loss) is a performance metric for evaluating the predictions of probabilities of membership to a given class.

* The scalar probability between 0 and 1 can be seen as a measure of confidence for a prediction by an algorithm. Predictions that are correct or incorrect are rewarded or punished proportionally to the confidence of the prediction.

**Smaller log loss is better with 0 representing a perfect log loss.**

## 3. Area Under ROC Curve
* Area Under ROC Curve (or ROC AUC for short) is a performance metric for binary classification problems.

* The AUC represents a model’s ability to discriminate between positive and negative classes. An area of 1.0 represents a model that made all predictions perfectly. An area of 0.5 represents a model as good as random.

* A ROC Curve is a plot of the true positive rate and the false positive rate for a given set of probability predictions at different thresholds used to map the probabilities to class labels. The area under the curve is then the approximate integral under the ROC Curve.

* You can see the the AUC is relatively close to 1 and greater than 0.5, suggesting some skill in the predictions.

## 4. Confusion Matrix
* The confusion matrix is a handy presentation of the accuracy of a model with two or more classes.

* The table presents predictions on the x-axis and accuracy outcomes on the y-axis. The cells of the table are the number of predictions made by a machine learning algorithm.

* For example, a machine learning algorithm can predict 0 or 1 and each prediction may actually have been a 0 or 1. Predictions for 0 that were actually 0 appear in the cell for prediction=0 and actual=0, whereas predictions for 0 that were actually 1 appear in the cell for prediction = 0 and actual=1. And so on.

* Although the array is printed without headings, you can see that the majority of the predictions fall on the diagonal line of the matrix (which are correct predictions).

## 5. Classification Report
* Scikit-learn does provide a convenience report when working on classification problems to give you a quick idea of the accuracy of a model using a number of measures.

* The classification_report() function displays the precision, recall, f1-score and support for each class.

*You can see good prediction and recall for the algorithm.
