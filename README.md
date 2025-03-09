# Dealing with Imbalanced Dataset

## Overview
In this project, we analyze the **Credit Fraud dataset** and utilize various predictive models to determine the accuracy of detecting fraudulent transactions. The primary challenge is handling the **imbalanced dataset**, where fraudulent transactions are significantly fewer than normal transactions. We explore techniques such as **undersampling, oversampling, and ensemble methods** (e.g., Random Forest, XGBoost) to address this issue effectively.

## Goals
1. **Understand the Data Distribution**: Analyze the dataset to comprehend the imbalance and structure of fraud vs. non-fraud transactions.
2. **Create a Balanced Subset**: Generate a 50/50 sub-dataframe of fraudulent and non-fraudulent transactions.
3. **Evaluate Classifiers**: Compare multiple classification algorithms and determine which yields the highest accuracy.
4. **Assess Sampling Techniques**: Investigate the impact of **undersampling and oversampling** to determine the best approach.

---

## Learnings & Key Insights
- **Focus on Extreme Outliers**: Rather than removing all outliers, we emphasize extreme outliers to prevent information loss that could degrade model performance.
- **Perform Undersampling During Cross-Validation**: Conducting undersampling before cross-validation may lead to inconsistencies, as the same minority-class samples could appear in both training and test sets, leading to misleading results.
- **Limitations of Undersampling**: In our undersampled dataset, models often misclassify non-fraudulent transactions as fraudulent cases, which can reduce reliability in real-world scenarios.
- **Random Undersampling Considerations**: After oversampling, removing outliers can impact model performance; therefore, it is crucial to compare results with the test set to ensure effectiveness.

---

## Conclusion
The main objective is to ensure our models **accurately classify both fraudulent and non-fraudulent transactions** while mitigating the challenges of an imbalanced dataset. By leveraging **sampling techniques and ensemble models**, we aim to improve detection rates while minimizing false positives and false negatives. Further optimizations and advanced techniques can enhance predictive performance in real-world fraud detection applications.

Feel free to contribute or suggest improvements!
