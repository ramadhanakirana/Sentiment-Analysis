## What is sentiment analysis? 🤔
Sentiment analysis is a technique that works by classifying polarity in text contained in sentences to determine the class of sentiment labels that match the data. Thus, the results of sentiment analysis will describe emotional states such as joy, anger, or sadness.

## Methods and Data Sources
The method used in this analysis is to use a Support Vector Machine with data sourced from reviews of the JKN Mobile application on the Google Play Store from January 2 to February 2, 2023. The reviews taken are reviews with a rating of 1 and 2 for the negative class and a rating of 4 and 5 for the positive class. Rating 3 is not used because it is considered neutral.

## Evaluation Parameters
To evaluate a model, several evaluation parameters are usually used. This evaluation parameter is taken from the confusion matrix. The evaluation parameters are:
1. Accuracy (the proportion of the number of correct predictions): 
   $Accuracy = TP + TN / TP + TN + FP + FN$
3. Recall (the proportion of how often the model predicts a true positive):
   $Recall = TP / (FN + TP)$
5. Precision (the proportion when the actual class is positive, how often the model predict positive):
   $Precision = TP / (FP + TP)$
7. F1-Score (harmonic average of precision and recall)
   $F1-Score = 2.((precision.recall)/(precision + recall))$
9. AUC (evaluate the extent to which the model can discriminate between positive and negative reviews):
    $AUC = 0.5 x ((TP / (TP + FN)) + (TN / (TN + FP)))$
    

## Kesimpulan 📃
Berdasarkan analisis yang telah dilakukan (syntax pengerjaan terlampir), maka dapat disimpulkan seperti berikut:


