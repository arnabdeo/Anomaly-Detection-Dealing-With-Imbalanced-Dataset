# Dealing-With-Imbalanced-Dataset

Here we will be dealing with Credit Fraud dataset, here we will use various predictive models to see how accurate they are in detecting whether a transaction is a normal payment or a fraud. 
The main objective is to find handle the imbalance dataset. Though this can be easily handled by Ensemble methods like Random Forest, XGBoost etc.

Our Goals:
*  Understand the distribution of data that was provided.
* Create a 50/50 sub-dataframe ratio of "Fraud" and "Non-Fraud" transactions.
* Determine the Classifiers we are going to use and decide which one has a higher accuracy.
* Comparing undersampling and oversampling which is to be preferred.

Learnings:
*  We want to focus more on "extreme outliers" rather than just outliers. Why? because we might run the risk of information loss which will cause our models to have a lower accuracy.
*  Undersampling to be perform while Cross Validation, not before that cause the same minority-class samples might end up in both the training and test sets or after cross-validating different folds may have different distributions, making the model learn from inconsistent patterns.
*  In our undersample data our model is unable to detect for a large number of cases non fraud transactions correctly and instead, misclassifies those non fraud transactions as fraud cases.

Random Undersampling is covered, one can calculate the accuracy after removing the outliers after oversampling and compare it with test set.


The main thing is to see if our models are able to correctly classify no fraud and fraud transactions.
