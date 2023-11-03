# credit-risk-classification

CREDIT RISK ANALYSIS REPORT
This report describe the purpose, score and results of the machine learning that i build in the code.

PURPOSE OF THE ANALYSIS

The purpose of the analysis is to compare two Logistic Regression model to predict the risk classification of diffferent loans. the variable y, the labels, we have the classification (0 is a healthy loan and 1 is high-.risk loan). The first model, use the original database that is not balance between healthy and high risk loans. If you check the data, you can see that the database have 75063 healthy loans and 2500 high-risk loans. 

In the second model, we use the RandomOVerSampler module from the imbalanced-learn library to resample the data. this is to "create" a database from the original but the module add the necessary samples for the minority class.

SCORES OF THE MACHINE LEARNING MODEL

If we see the classification report from both model (original and resampled model) we have that the accuracy the higher than to 95% in both cases (95% in the origianl model and 99% in resampled model) so we can say that both model make well predictions. 

Also, the presicion in the resampled model is over 99% and in the original model is 100%w to the healthy loans. when you see the high-risk loans, in the original model the precision is 85% but increase to 99% when you resampled the data.

Moreover, the recall in both models is over 90% (for high risk loans, 91% with the original model and 99% with the resampled data), sufficient to trust in both model. 

in the case of original data, we can see a difference between healthy loans and high risk loans. This can be explained because the original database is unbalance, having much more healthy loans than high risk loans so you can conclude that the predictions to high risk loans can have lower accuracy. however, when we used the resampled data, this difference disappear.

RESULT OF THE MACHINE LEARNING MODEL

The results of this analysis shows that we can trust in the model, with or without balance data, having a balanced accuracy over 90% in both models. Also, if you can see the confusion matrix, in both case you can see that in most cases, you can find that the model make good predictions.