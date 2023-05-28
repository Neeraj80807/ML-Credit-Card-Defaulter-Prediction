# Credit Card Defaulter Prediction

This repository contains a dataset and code for performing credit card defaulter prediction using machine learning techniques. The dataset (`Default_Fin.csv`) is a synthetic dataset created from actual financial data, modified for academic purposes.

## Dataset Description
The dataset contains the following columns:
- `index`: Serial number or unique identifier of the loan taker.
- `Employed`: Boolean value indicating employment status (1 = employed, 0 = unemployed).
- `Bank Balance`: Bank balance of the loan taker.
- `Annual Salary`: Annual salary of the loan taker.
- `Defaulted?`: Boolean value indicating loan default status (1 = defaulted, 0 = not defaulted).

## Setup and EDA
To set up the dataset for exploratory data analysis (EDA), follow these steps:
1. Download the `Default_Fin.csv` file from this repository.
2. Load the dataset into your preferred programming environment or tool.
3. Perform EDA tasks such as checking for missing data, handling duplicates, and exploring data distributions using count plots, histograms, pair plots, and correlation plots.
4. Split the data into training and test datasets (75% training, 25% test or validation) to prepare for model training and evaluation.
5. Apply feature scaling techniques if necessary.

## Upsampling with SMOTE
As part of the EDA, it was observed that defaulted cases represented only about 3% of the samples, indicating an imbalanced dataset. To address this, we applied the Synthetic Minority Oversampling Technique (SMOTE) to upsample the minority class and rebalance the dataset.

## Model Building and Evaluation
We built three classification models on the dataset:
- Logistic Regression
- Random Forest Classifier
- Naive Bayes Classifier

For each model, we measured the errors and accuracy. To find the optimal values for the depth and number of trees in the random forest, we used GridSearchCV, which performed a grid search with cross-validation to propose the best hyperparameters.

## Visualizing Model Performance
To gain insights into the performance of the models, visualizations such as confusion matrices, ROC curves, and precision-recall curves were generated. These visualizations provide a comprehensive understanding of the models' predictive capabilities and help evaluate their performance.

Please refer to the code files in this repository for detailed implementation and further instructions on running the analysis.

Note: This dataset and code are intended for educational purposes and serve as a starting point for beginners interested in financial analytics and credit card defaulter prediction.
