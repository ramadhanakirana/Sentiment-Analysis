## What is sentiment analysis? 🤔
Sentiment analysis is a technique that works by classifying polarity in text contained in sentences to determine the class of sentiment labels that match the data. Thus, the results of sentiment analysis will describe emotional states such as joy, anger, or sadness.

## Methods and Data Sources ⚙️
The method used in this analysis is to use a Support Vector Machine with data sourced from reviews of the JKN Mobile application on the Google Play Store from January 2 to February 2, 2023. The reviews taken are reviews with a rating of 1 and 2 for the negative class and a rating of 4 and 5 for the positive class. Rating 3 is not used because it is considered neutral.

## Evaluation Parameters 👇
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
    $AUC = 0.5((TP / (TP + FN)) + (TN / (TN + FP)))$
    

## Conclusion 📃
Based on the analysis that has been carried out (the working syntax is attached), it can be concluded as follows:
1. The best parameters for SVM are C = 10 for Linear SVM and C = 10 and gamma = 1 for RBF SVM.
2. Linear SVM has an accuracy value of 0.9085, recall of 0.7482, precision of 0.8992, F1 Score of 0.8168, and AUC of 0.8584.
3. RBF SVM has an accuracy value of 0.9238, recall of 0.8110, precision of 0.8655, F1 Score of 0.8374, and AUC of 0.8854.
4. From points (2) and (3) above, it can be concluded that the RBF kernel SVM is better used to classify JKN Mobile application review sentiment.
5. From the existing reviews, we got wordcloud for positive and negative sentiments as follows
   ![image](https://github.com/ramadhanakirana/analisissentimen/assets/102908444/f2b290ff-3433-4ba8-a6e4-dbf994eb04c9)
From the image above, for positive sentiment, it can be seen that the words 'good (bagus)' and 'easy (mudah)' dominate in the visualization. Apart from the expression that the application is good and easy to use, it can be concluded that the JKN Mobile application has helped serve the community by making changing health facilities (FASKES) easier, providing good service and a fast response, and meeting expectations from users so that the JKN Mobile application continues to improve its services.
   ![image](https://github.com/ramadhanakirana/analisissentimen/assets/102908444/8d0ea202-a626-46bb-ad0b-ddec4f300ce6)
The negative sentiment from users can be seen in the image above, which is a word cloud visualization image with negative sentiment. It can be seen that the words 'access' and 'impractical' dominate in the visualization. So that through you can, it was concluded that the JKN Mobile application received negative sentiment from users, including the appearance of inappropriate access hours, impractical registration, applications after updating that cannot be opened, and the One-Time Password (OTP) code must be used.
