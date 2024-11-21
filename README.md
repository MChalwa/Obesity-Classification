# Obesity Levels Classification Model
## Project Overview
This repository showcases a machine learning model developed to classify obesity levels based on various health features, including eating habits, physical activity, and lifestyle factors. 
The dataset used for training includes information on factors like frequent calorie consumption, physical activity, and alcohol use, with the target variable representing different obesity categories: Underweight, Normal, Overweight, Obesity I, Obesity II, and Obesity III.
The project involved extensive data preprocessing, including Exploratory Data Analysis (EDA), outlier detection, and feature scaling. Dummy variables were created for categorical features, and the data was split into training and test sets. Several classification algorithms were evaluated, including Random Forest, Decision Tree, and Gradient Boosting.

After applying cross-validation and evaluating the model on the test set, the model achieved an accuracy of approximately 95%. Precision, recall, and F1-score metrics were also computed, revealing strong performance across all obesity categories, particularly in extreme obesity classes.

This model can serve as a useful tool for identifying obesity levels, enabling early intervention and targeted public health programs. It demonstrates how machine learning can be applied to health-related datasets for predictive analytics and health monitoring.
## Key Insights from the Model Output
### 1. Accuracy
The model achieved a high accuracy of 94.56% on the test set, which indicates that it is effectively predicting obesity categories based on the features (e.g., eating habits, physical condition, lifestyle, etc.).
This high accuracy suggests that the model can reliably categorize individuals into the appropriate obesity classes (Underweight, Normal, Overweight, Obesity I, Obesity II, Obesity III).
### 2. Precision, Recall, and F1-Score
Looking at the classification report,the following were observed for each obesity class (0: Underweight, 1: Normal, 2: Overweight, etc.):

- Precision: The model's ability to correctly identify a class when it predicts that class. For example, the precision for class 0 (Underweight) is 0.98, which means that when the model predicts a person is underweight, it is correct 98% of the time.
- Recall: The model's ability to correctly predict all instances of a class. For example, recall for 1 (Normal) is 0.90, which means 90% of all actual normal individuals were correctly predicted.
- F1-Score: A balance of precision and recall. A higher F1-score indicates a better model that balances both false positives and false negatives.
- The macro avg and weighted avg gives an overall measure of model performance, considering all classes, which are both around 0.94. This is quite strong, meaning the model is doing well across all obesity categories.
### 3. Observations per Class
The model performed particularly well for classes 0 (Underweight), 4 (Obesity I), and 5 (Obesity II), with near-perfect precision and recall (1.00), which shows that the model can predict these categories very reliably.
Classes 1 (Normal) and 6 (Obesity III) have slightly lower recall, which may indicate some instances of misclassification in these categories (e.g., normal individuals being misclassified as obese, or vice versa).
## Actionable Insights
- Identifying At-Risk Groups: The model's ability to correctly predict obesity levels means it could be used to identify individuals who are at risk of developing obesity or who are already obese. Public health interventions can focus on those classified in higher obesity categories (Obesity I, II, III).

- Early Intervention: For individuals identified as underweight or overweight, the model can help pinpoint early stages of potential health risks, allowing for early intervention in nutrition or exercise regimes.

- Targeted Health Programs: The model could help in designing targeted health programs or campaigns that focus on individuals in specific obesity categories, such as Obesity III (severe obesity), who may require more intensive interventions.
## Conclusion
The obesity classification model developed for predicting obesity levels based on individuals' health data, eating habits, and physical activity shows strong performance, with an accuracy of 94.56% on the test set. The model performs exceptionally well in identifying individuals in extreme obesity categories (Underweight, Obesity I, Obesity II), and provides a reliable tool for assessing the risk levels of individuals based on their health behaviors. This can be particularly valuable for public health initiatives aimed at early intervention and targeted programs for obesity prevention. However, slight misclassifications in the Normal and Obesity III categories suggest that future model refinements or additional features could further enhance performance.

