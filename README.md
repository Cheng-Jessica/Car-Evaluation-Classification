# Car-Evaluation-Classification

## Overview
This GitHub repository contains the code and data for a machine learning project focused on car evaluation classification. The goal of this project is to explore and compare different classification techniques, such as Decision Tree, K-Nearest Neighbors (KNN), Logistic Regression, Support Vector Machine (SVM), and Naive Bayes. The dataset used for this project includes 1728 records, each representing a car evaluation based on various attributes.

## Dataset (http://archive.ics.uci.edu/ml/datasets/Car+Evaluation)
The dataset used in this project is obtained from the UCI Machine Learning Repository and includes seven attributes: buying price, maintenance price, number of doors, capacity in terms of persons, size of luggage boot, estimated safety, and the evaluation of the car (unacceptable, acceptable, good, very good). The attributes are preprocessed and transformed into a binary format, and the target variable is encoded into numerical values.

## Project Structure
The project is organized into the following sections:

1. Data Loading and Exploration: The dataset is loaded, and exploratory data analysis is performed to understand the structure of the data.

2. Data Preprocessing: Categorical variables are converted into binary format, and the target variable is encoded into numerical values. Feature scaling is applied to standardize the input variables.

3. Class Imbalance Handling: The target variable is oversampled using the Synthetic Minority Over-sampling Technique (SMOTE) to address class imbalance.

4. Classification Models: Different classification models, including Decision Tree, KNN, Logistic Regression, SVM, and Naive Bayes, are implemented and tuned using GridSearchCV for hyperparameter optimization.

5. Model Evaluation: Models are evaluated using Matthews Correlation Coefficient (MCC) as the performance metric. Confusion matrices and classification reports are generated for detailed evaluation.

6. Numeric (Ordinal) Variables Experiment: The dataset is reprocessed to treat ordinal variables as numerical, and the same classification models are re-evaluated.

## Results
The average MCC scores for each classification model are as follows:
|Model Types| Treated as categorical (Binary format) Mean MCC | Treated as numerical (Ordinal) Mean MCC |
|-----------|------------------|-----------|
|Decision Tree | 0.88 | 0.81 |
|K-NN | 0.97 | 0.95|
|Logistic Regression | 0.85 | 0.81 |
|SVM Classification | 0.99 | 0.97 |
|Naive Bayes | 0.64 | 0.64 |


## Instructions for Reproduction
- Clone this repository to your local machine.
- Ensure you have the required Python libraries installed by running pip install -r requirements.txt.
- Execute the Jupyter Notebook files in sequential order to reproduce the analysis.


Feel free to explore and modify the code to further investigate specific aspects of the project or test additional models. Your feedback and contributions are welcomed!
