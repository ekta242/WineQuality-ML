# Wine Quality Prediction

A machine learning project to predict wine quality using a Random Forest Classifier, built during my Data Science & Machine Learning internship at DeltaQ Solutions.

## Overview

This project explores how well a Random Forest model can classify wine quality based on physicochemical properties of the wine (e.g. acidity, sugar content, pH, alcohol level — update with the actual features you used). Alongside building the model, the focus was on understanding *why* the model behaves the way it does, not just getting a number out.

## Approach

- **Model:** Random Forest Classifier
- **Preprocessing:**
  - IQR-based outlier removal to clean the dataset before training
  - SMOTE (Synthetic Minority Oversampling Technique) to address class imbalance in the quality labels
- **Evaluation:** Train/test split with accuracy as the primary metric

## Results

| Metric | Accuracy |
|---|---|
| Training | ~1.00 |
| Testing | 0.93 |

The training accuracy is close to perfect, which is a classic sign of overfitting in Random Forest models — the model has effectively memorized patterns in the training data rather than purely learning generalizable rules. The testing accuracy of 0.93 shows the model still generalizes reasonably well despite this, but the gap is worth noting rather than ignoring.

## Tech Stack

- Python
- scikit-learn
- pandas / numpy

## Dataset
 Datset was provided by the internship 

---
Part of a series of three classification projects (Wine Quality, Liver Disease, Diabetes Prediction) completed during my internship at DeltaQ Solutions, June 2026.