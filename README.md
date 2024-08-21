### neural-network-challenge-1
## Module 18 homework
# Leigh Nash
# Project Overview
 - source:  Chatgpt
# This project uses TensorFlow's Keras API to build a neural network model that predicts whether a student is likely to successfully repay their loan. The model is trained on a dataset with multiple features related to students' academic and financial background.

## Data Preparation

1. **Data Import**: The dataset (`student-loans.csv`) is read into a Pandas DataFrame.
2. **Feature and Target Selection**: 
    - **Features (X)**: All columns except `credit_ranking`.
    - **Target (y)**: `credit_ranking` column.
3. **Data Splitting**: The data is split into training and testing sets using `train_test_split`.
4. **Scaling**: Features are scaled using Scikit-learn's `StandardScaler`.
## Saving and Loading the Model

- The trained model is saved as `student_loans.keras`.
- The model can be reloaded for future predictions using TensorFlow's `load_model` function.

## Prediction and Analysis
- The model is used to make predictions on the test data.
- Predictions are saved to a DataFrame and rounded to binary values (0 or 1).
- A classification report is generated to compare predictions against actual test labels
