# BMIF 802 Lab 7: Classification 2 — Tuning, Neural Networks, and Model Explanation

## Description

In this lab, you will continue working with the Cleveland Heart Disease dataset from Lab 6. You will reuse your Lab 6 preprocessing, train several classification models, tune important parameters, compare models using classification metrics, build a small fully connected neural network, and use SHAP values to help explain the neural network predictions.

1. Start with the same cleaned/preprocessed dataset workflow from Lab 6.
2. Reuse the classification models from Lab 6.
3. Add a Support Vector Machine model.
4. Compare models using confusion matrices, precision, recall, F1-score, MCC, ROC curves, and AUC.
5. Tune Random Forest and SVM models using both grid search and random search.
6. Build and train a small fully connected neural network using Keras.
7. Run the neural network on a regular laptop CPU and then repeat the workflow in Google Colab with a GPU.
8. Use SHAP values to interpret which features push the neural network output toward or away from the positive class.

## Learning objectives

By the end of this lab, you should be able to:

- Explain why SVM models are sensitive to feature scaling.
- Train and evaluate an SVM classifier.
- Use `GridSearchCV` and `RandomizedSearchCV` for hyperparameter tuning.
- Tune more than one parameter at a time for Random Forest and SVM models.
- Interpret common binary classification metrics: accuracy, precision, recall, F1-score, MCC, ROC curve, and AUC.
- Build a simple fully connected neural network for binary classification.
- Train the neural network on CPU and understand how the same code can use a GPU in Google Colab.
- Perform a small neural network parameter search.
- Use SHAP values to explain neural network predictions.

## Packages used

This lab uses the same general course environment plus a few machine learning packages:

```bash
pip install pandas numpy matplotlib scikit-learn scipy tensorflow shap
```

Notes:

- `tensorflow` is used for the fully connected neural network.
- `shap` is used for model explanation.
- In Google Colab, `tensorflow` is usually already available, but `shap` may need to be installed.

## Dataset

This lab reuses the Cleveland Heart Disease dataset from Lab 6.

Expected file location:

```text
data/heart_disease_cleveland.csv
```

## Checklist

Students should work through the lab in this order:

- [ ] Open the student notebook.
- [ ] Confirm that the Cleveland Heart Disease dataset loads correctly.
- [ ] Reuse or rebuild the preprocessing workflow from Lab 6.
- [ ] Train the Lab 6 classification models again.
- [ ] Add an SVM classifier.
- [ ] Compare all models using multiple classification metrics.
- [ ] Plot and interpret at least one confusion matrix.
- [ ] Plot and interpret ROC curves.
- [ ] Tune a Random Forest using grid search.
- [ ] Tune a Random Forest using random search.
- [ ] Tune an SVM using grid search.
- [ ] Tune an SVM using random search.
- [ ] Build and train a fully connected neural network using Keras.
- [ ] Tune at least three neural network settings.
- [ ] Run the neural network notebook in Google Colab.
- [ ] Check whether Colab is using a GPU.
- [ ] Generate SHAP values for the neural network.
- [ ] Write a short interpretation of which features appear important.
