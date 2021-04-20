# Metrics_to_Evaluate
Machine Learning - Classification Metrics, Regression Metrics


## Classification Metrics:
## How to use the following metrics:

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

* You can see good prediction and recall for the algorithm.

![Classification Report](https://user-images.githubusercontent.com/62986688/115344047-641cb200-a1ca-11eb-9d2c-b1e5f0c74534.png)


## Regression Metrics:
## How to use the following metrics:

1. Mean Absolute Error.
2. Mean Squared Error.
3. R^2.

## 1. Mean Absolute Error
* The Mean Absolute Error (or MAE) is the average of the absolute differences between predictions and actual values. It gives an idea of how wrong the predictions were.

* The measure gives an idea of the magnitude of the error, but no idea of the direction (e.g. over or under predicting).

* A value of 0 indicates no error or perfect predictions.

* Like logloss, this metric is inverted by the cross_val_score() function.

## 2. Mean Squared Error
* The Mean Squared Error (or MSE) is much like the mean absolute error in that it provides a gross idea of the magnitude of error.

* Taking the square root of the mean squared error converts the units back to the original units of the output variable and can be meaningful for description and presentation. 

* This is called the Root Mean Squared Error (or RMSE).

* This metric too is inverted so that the results are increasing.

## 3. R^2 Metric
* The R^2 (or R Squared) metric provides an indication of the goodness of fit of a set of predictions to the actual values. In statistical literature, this measure is called the coefficient of determination.

* This is a value between 0 and 1 for no-fit and perfect fit respectively.

* You can see that the predictions have a poor fit to the actual values with a value close to zero and less than 0.5.

# Summary
## You learned about 3 classification metrics:

Accuracy.

Log Loss.

Area Under ROC Curve.

## Also 2 convenience methods for classification prediction results:
Confusion Matrix.

Classification Report.

## And 3 regression metrics:
Mean Absolute Error.

Mean Squared Error.

R^2.
