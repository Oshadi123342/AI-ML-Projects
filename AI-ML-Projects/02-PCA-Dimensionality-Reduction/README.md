# 📉 PCA Dimensionality Reduction

![PCA](https://img.shields.io/badge/Technique-PCA-8A2BE2) ![Variance](https://img.shields.io/badge/Retained%20variance-%E2%89%A595%25-teal) ![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange)

## 🎯 Objective
Reduce the dimensionality of an already-preprocessed lung cancer classification dataset while retaining at least 95% of training-data variance.

## 🛠 Workflow

1. Load `data/train_selected_features.csv` and `data/test_selected_features.csv`.
2. Separate `LUNG_CANCER` from the input features.
3. Fit `PCA(n_components=0.95, random_state=42)` on training features **only**.
4. Transform the training and test features with the same PCA model.
5. Visualize individual and cumulative explained variance.
6. Export transformed datasets to `results/outputs/`.

## 📊 Recorded outcome

The notebook reports **8 principal components** selected to reach the 95% explained-variance threshold. That number depends on the input datasets.

## ▶️ Run

Install dependencies from the root `requirements.txt`. Run `PCA_Dimensionality_Reduction.ipynb` with this project folder as the working directory, after adding your own:

```text
data/train_selected_features.csv
data/test_selected_features.csv
```

Both files must contain a `LUNG_CANCER` target column and matching numeric feature columns. Generated files are saved to `results/outputs/` and `results/eda_visualizations/`. The input datasets are not provided in this package.

> The original notebook's relative paths were adapted to this standalone project layout. Existing notebook outputs are retained, but the notebook has not been rerun.
