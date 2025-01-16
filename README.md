# Vacation Preference Prediction using Machine Learning

## Overview

This project leverages machine learning to predict vacation preferences—whether individuals prefer mountains or beaches—based on demographic and lifestyle data. By analyzing a dataset of over 52,000 individuals, this project aims to uncover insights and build predictive models to assist the tourism and travel industry in offering personalized recommendations.

## Objectives

- **Data Analysis**: Explore trends and relationships in the dataset.
- **Model Development**: Train various machine learning models to predict vacation preferences.
- **Feature Insights**: Identify key demographic and lifestyle factors influencing preferences.
- **Deployment**: Develop a model that can be used by businesses for targeted marketing.
- **Educational Value**: Gain practical experience with data mining and machine learning.

## Dataset

The dataset contains 52,444 entries and 13 features, including:
- **Age**
- **Gender**
- **Income**
- **Education Level**
- **Travel Frequency**
- **Vacation Budget**
- **Location Type** (Urban/Suburban/Rural)
- **Proximity to Mountains and Beaches**
- **Environmental Concerns**
- **Pets Ownership**
- **Preferred Activities**
- **Favorite Season**

All features were preprocessed for efficient modeling, including handling categorical data and normalizing numerical features.

## Methodology

1. **Data Preprocessing**:
   - Inspected and cleaned the dataset.
   - Encoded categorical variables.
   - Normalized numerical features for model compatibility.

2. **Feature Selection**:
   - Analyzed correlations to remove redundant features.
   - Used Recursive Feature Elimination (RFE) to identify the most significant predictors.

3. **Model Training**:
   - Evaluated multiple models using 9-fold cross-validation:
     - Logistic Regression
     - Decision Trees
     - Random Forest
     - Support Vector Machines
     - Naive Bayes
     - K-Nearest Neighbors
   - Hyperparameter tuning was conducted using grid search for each model.

4. **Evaluation**:
   - Assessed models based on accuracy, precision, recall, and F1-score.
   - Visualized learning curves, ROC-AUC, and confusion matrices for in-depth analysis.

5. **Deployment**:
   - Selected Logistic Regression as the best-performing model based on accuracy and retrained it on the full dataset.

## Results

| Model                  | Test Accuracy | Precision | Recall | F1-Score |
|------------------------|---------------|-----------|--------|----------|
| Logistic Regression    | 100.00%      | 100.00%   | 100.00%| 100.00%  |
| Decision Tree          | 99.71%       | 99.71%    | 99.71% | 99.71%   |
| Random Forest          | 99.85%       | 99.85%    | 99.85% | 99.85%   |
| Support Vector Machine | 99.98%       | 99.98%    | 99.98% | 99.98%   |
| Naive Bayes            | 75.21%       | 87.54%    | 75.21% | 76.86%   |
| K-Nearest Neighbors    | 97.16%       | 97.17%    | 97.16% | 97.16%   |

Logistic Regression emerged as the top model, achieving perfect accuracy on the test set.

## Key Learnings

- Feature engineering and preprocessing are critical for model success.
- Hyperparameter tuning significantly improves model performance.
- Logistic Regression, despite its simplicity, can outperform complex models with well-prepared data.

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/bedirhankaraahmetli/Vacation-Preferences.git
