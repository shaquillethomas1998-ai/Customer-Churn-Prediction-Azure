# Customer Churn Prediction — Azure Machine Learning

A coursework project by Shaquille Thomas using Azure Machine Learning Designer to build and evaluate a baseline customer churn classifier.

## Purpose

Explore customer churn prediction through a visual machine learning workflow, from data preparation to model evaluation.

## Tools

Azure Machine Learning Designer · Logistic Regression

## Workflow

1. Handle missing values.
2. Select columns and adjust metadata.
3. Encode categorical variables.
4. Split the data into training and test sets.
5. Train a two-class logistic regression model.
6. Score the test data and evaluate predictions.
7. Convert scored results to CSV.

## Evaluation Results

At a classification threshold of 0.5:

| Metric | Result |
|---|---:|
| Accuracy | 66.5% |
| Precision | 60.7% |
| Recall | 23.3% |
| F1 score | 0.337 |
| ROC AUC | 0.649 |

The evaluation contains 200 test cases: 17 true positives, 11 false positives, 56 false negatives and 116 true negatives.

## Interpretation

The model identified 17 of 73 positive cases. Its low recall shows that many positive cases were missed at the default threshold.

Predicting every case as negative would achieve 63.5% accuracy on this test set. The model's 66.5% accuracy therefore represents a modest improvement over that simple baseline.

## Potential Improvements

- Verify the target label and review input features for leakage.
- Fit learned preprocessing steps using training data only.
- Compare alternative models using cross-validation.
- Explore classification thresholds using validation data.
- Evaluate the trade-off between missed churn cases and unnecessary retention outreach.

These are proposed improvements, not completed work.

## Repository Contents

Three screenshots document data preparation, model training and evaluation results.

This repository is a visual project case study. It does not currently include an executable pipeline export, source dataset or deployed prediction endpoint.

## Limitations

These results describe one coursework experiment and do not establish readiness for business use. Further validation and improved positive-case detection would be needed.
