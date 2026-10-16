# 🫁 Lung Cancer Prediction Using KNN

![ML](https://img.shields.io/badge/Machine%20Learning-Classification-blueviolet) ![KNN](https://img.shields.io/badge/Algorithm-KNN-orange) ![Python](https://img.shields.io/badge/Language-Python-blue)

## 🎯 Objective
Explore binary lung cancer classification with a K-Nearest Neighbors (KNN) model using a synthetic lung cancer CSV dataset. **This notebook is educational and is not a validated medical tool.**

## 🛠 Workflow

1. Load `data/lcs_synthetic_20000.csv`.
2. Encode gender, binary symptom columns, and target labels.
3. Split into stratified training (80%) and testing (20%) sets.
4. Standardize features using the training-fitted scaler.
5. Compare baseline KNN with cross-validated hyperparameter searches.
6. Evaluate accuracy, precision, recall, F1, ROC AUC and confusion matrix.
7. Plot KNN decision boundaries using two PCA components.

## 📊 Notebook results

| Experiment | Test accuracy |
|---|---:|
| Default KNN (`k=5`) | 86.05% |
| Grid search over `k=1..20` | 87.15% |
| Grid search over `k`, weights and distance metrics | 87.15% |

**Selected hyperparameters:** `n_neighbors=17`, `weights='uniform'`, `metric='euclidean'`. Reported precision: `0.87`, recall: `1.00`, F1: `0.93`, ROC AUC: `0.52` (rounded). High recall and accuracy alone do not establish good discrimination; examine imbalance and all metrics.

## ▶️ Run

From this folder, place your dataset at `data/lcs_synthetic_20000.csv` and run `Lung_Cancer_KNN.ipynb` using Jupyter. Install packages from the root `requirements.txt` first. The CSV is **not included**. Make sure its columns match those used in the notebook.

> The notebook's original absolute Windows dataset path has been replaced with a project-relative path. Saved outputs are from the uploaded notebook, not a fresh execution.
