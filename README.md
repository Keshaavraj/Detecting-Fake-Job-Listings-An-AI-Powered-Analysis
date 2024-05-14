# Detecting Fake Job Postings: A Machine Learning Approach

## Objective:

This project aims to develop a machine-learning model capable of distinguishing between fake and legitimate job postings. To achieve this, the code aims to:

1. **Preprocess Data:** Prepare the dataset by cleaning and selecting relevant features.
2. **Model Selection:** Evaluate various classification algorithms to identify the most suitable model for the task.
3. **Model Evaluation:** Assess the performance of the chosen model using cross-validation and train-test splits.
4. **Feature Importance:** Determine the importance of features in predicting job fraudulence.
5. **Interpretability:** Enhance model interpretability by explaining individual predictions using LIME.

## Description:

The Python script provided orchestrates a sequence of operations aimed at the classification of job postings as either genuine or fraudulent. It begins by importing necessary libraries and proceeds through data loading, feature selection, data standardization, model evaluation, model selection, train-test splitting, model training and evaluation, performance metrics calculation, feature importance analysis, and model interpretability enhancement.

## Code Explanations:

Each section of the code is meticulously described, covering tasks such as data preprocessing, model evaluation, model selection, train-test splitting, model training, performance metric calculation, feature importance analysis, and model interpretability.

## Findings:

1. Choice of model and train-test split significantly influences classification performance.
2. Logistic Regression exhibits consistent performance across different splits.
3. Certain features exert more influence on the classification task than others.
4. LIME explanations provide valuable insights into individual predictions, enhancing model interpretability.

## Evaluation Metrics and LIME Explanations:

### Model Evaluation:

- Dummy Classifier (Baseline Accuracy):
    - Mean Accuracy: 0.760 (0.000)
- Classification Models (Cross-Validation):
    - SVM: 0.859 (0.034)
    - Logistic Regression: 0.863 (0.034)
    - KNN: 0.835 (0.038)
    - Bagging: 0.850 (0.034)
    - Random Forest: 0.860 (0.032)
    - Extra Trees: 0.858 (0.032)

### Logistic Regression Model:

- Logistic Regression Accuracy (80/20 Split):
    - Accuracy: 0.869
- Logistic Regression Accuracy (70/30 Split):
    - Accuracy: 0.867
- Logistic Regression Accuracy (67/33 Split):
    - Accuracy: 0.864

### SVM Model:

- SVM Accuracy (80/20 Split):
    - Accuracy: 0.865
- SVM Accuracy (70/30 Split):
    - Accuracy: 0.870
- SVM Accuracy (67/33 Split):
    - Accuracy: 0.864

### LIME Explanations:

- Feature Importances (Random Forest Model):
    - Features: ['Experience', 'Salary', 'Reviews', 'Age_of_post_in_days', 'Company_Logo_Present', 'Rating', 'topic0', 'topic1', 'topic2', 'topic3']
- LIME Explanation Summary:
    - Total Features: 10
    - Total Feature Importance Sum: 1.0

## Conclusion:

The provided code offers a comprehensive analysis of job fraudulence detection using machine learning techniques. By evaluating various models, understanding feature importance, and enhancing interpretability, it assists in making informed decisions regarding fake job identification.
