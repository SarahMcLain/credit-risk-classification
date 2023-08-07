# credit-risk-classification

## Objective

The aim of this analysis was to develop a predictive model capable of classifying loans as either high-risk (class 1) or healthy (class 0). After the initial training process on the original data, the data was resampled using RandomOverSample from the imbalance-learning library to imporve the model's predictive accuracy. To evaluate the model's performance, we use key metrics such as precision, recall, and F1-score.

## Results

### Original Data:

* Precision for class 0: 1.00 (100% of the predicted healthy loans were actually healthy)
* Precision for class 1: 0.87 (87% of the predicted high-risk loans were actually high-risk)
* Recall for class 0: 1.00 (100% of the actual healthy loans were correctly predicted as healthy)
* Recall for class 1: 0.89 (89% of the actual high-risk loans were correctly predicted as high-risk)
* F1-score for class 0: 1.00 (mean of precision and recall for class 0)
* F1-score for class 1: 0.88 (mean of precision and recall for class 1)

### Resampled Data:

* Precision for class 0: 1.00 (100% of the predicted healthy loans were actually healthy)
* Precision for class 1: 0.87 (87% of the predicted high-risk loans were actually high-risk)
* Recall for class 0: 1.00 (100% of the actual healthy loans were correctly predicted as healthy)
* Recall for class 1: 1.00 (100% of the actual high-risk loans were correctly predicted as high-risk)
* F1-score for class 0: 1.00 (mean of precision and recall for class 0)
* F1-score for class 1: 0.93 (mean of precision and recall for class 1)

## Observations

In our evaluation of the model's performance on both the original and resampled datasets, we observed consistently high precision and recall scores overall. However, resampling the data significantly improved the model's predictive accuracy for assessing class 1 (high risk) loans; improving the recall of class 1 from 89% to 100% and increasing the f1-score by 5%. These findings indicate that resampling the data had a positive impact on the model's predictive power.

## Conclusion

While the model's predictions on the original data were already relatively accurate, this analysis underscores the substantial benefits of resampling our data. It demonstrates how resampling can effectively improve a model's performance, particularly in cases where class imbalance poses a challenge. This model is precise and accurate and can be safely used to predict whether or not a loan is healthy.