# credit-risk-classification

This GitHub repository contains a Python project that demonstrates the process of building a logistic regression model to predict loan statuses using machine learning techniques. The project is divided into several steps, as outlined below:

## Step 1: Data Preparation
- Import the necessary Python libraries, including `numpy`, `pandas`, and `pathlib`.
- Load the loan dataset from the "lending_data.csv" file in the "Resources" folder into a Pandas DataFrame.
- Separate the labels (y) and features (X) from the dataset.

## Step 2: Data Exploration
- Check the balance of the labels variable (y) by using the `value_counts` function.

## Step 3: Data Splitting
- Split the dataset into training and testing datasets using the `train_test_split` function from scikit-learn.

## Step 4: Building the Initial Logistic Regression Model
- Instantiate a logistic regression model with the `LogisticRegression` module from scikit-learn.
- Fit the model using the training data.
- Save the predictions on the testing data labels and evaluate the model's performance using metrics like accuracy, a confusion matrix, and a classification report.

## Step 5: Logistic Regression with Resampled Data
- Use the RandomOverSampler from the imbalanced-learn library to resample the training data, ensuring equal representation of both classes.
- Train a logistic regression model with the resampled data.
- Make predictions using the testing data and evaluate the model's performance.

## Model Evaluation
- For both the initial and resampled logistic regression models, we assess their performance using metrics such as balanced accuracy, confusion matrices, and classification reports.

## Conclusion
- The project provides answers to critical questions regarding the model's performance, including how well it predicts healthy (0) and high-risk (1) loans.

### Model Performance Summary
- The logistic regression model, trained with oversampled data, performs exceptionally well in predicting both healthy (label 0) and high-risk (label 1) loans. It achieves high precision, recall, and balanced accuracy scores for both categories, indicating accurate predictions for both types of loans.

