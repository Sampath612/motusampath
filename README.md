Comparing K-Fold and Stratified K-Fold Cross-Validation

## Overview
This project demonstrates the difference between K-Fold and Stratified K-Fold cross-validation techniques using the Breast Cancer Wisconsin Diagnostic dataset. It evaluates how each splitting strategy affects model accuracy and the distribution of class labels across the folds.

## Dataset
- Source: sklearn.datasets.load_breast_cancer()
- Type: Classification
- Features: 30 numerical input features
- Target Classes:
  - 0 = Malignant
  - 1 = Benign

## Methodology
- Model Used: Logistic Regression (sklearn.linear_model.LogisticRegression)
- Validation Techniques:
  - K-Fold (with shuffling, 5 splits)
  - Stratified K-Fold (with shuffling, 5 splits)
- Process:
  - Train and test the model on each fold
  - Calculate accuracy
  - Analyze class distribution within each test fold
## Visualizations
- Boxplot comparing the accuracy scores of K-Fold and Stratified K-Fold.
- Bar plot showing the class distribution across folds to highlight the benefit of using stratified splitting.

## Results Summary
- Stratified K-Fold maintains a more balanced distribution of class labels across folds.
- It generally results in more stable accuracy measurements, particularly important for imbalanced datasets.

## Dependencies
- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn

Install dependencies using:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
