# ML-projects
A collection of Machine Learning and Data Science projects showcasing my skills in Python, predictive modeling, and data manipulation.

## Heart Disease Prediction

[Notebook](Heart_Disease_Prediction/heart_disease_prediction.ipynb) · Python, pandas, scikit-learn · 918 patient records, 11 features

- **Data cleaning:** 172 `Cholesterol` values and 1 `RestingBP` value are recorded as 0, which is impossible in a living patient. They are treated as missing and imputed with the training median.
- **No leakage:** the split comes first. Imputation, scaling and one-hot encoding sit inside a scikit-learn pipeline and are fit on training data only.
- **Model choice:** five classifiers compared with 5-fold cross-validation on the training set. Random Forest won (CV F1 0.864). Bernoulli Naive Bayes was close (0.859).
- **Final result:** scored once on the 30% test set (276 records): accuracy 0.88, F1 0.90.

This is a learning project on a public dataset, not a medical tool.

## Severity Prediction

[Notebook](Severity_Prediction/severity_prediction.ipynb) · an early exercise classifying attack severity on a small 200-row dataset.
