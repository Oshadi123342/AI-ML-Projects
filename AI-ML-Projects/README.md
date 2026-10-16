<div align="center">

# 🤖 AI & Machine Learning Projects

### 🧠 Predictive Modeling · 📊 Classification · 🎯 PCA · 🐍 Python

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Scikit--learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

*A collection of practical, notebook-based machine learning experiments.*

</div>

---

## 🚀 Projects at a glance

| 🔬 Project | 🎯 Focus | 🛠 Methods |
|---|---|---|
| [01 · Lung Cancer Prediction using KNN](./01-Lung-Cancer-Prediction-KNN/) | Binary classification | KNN, StandardScaler, GridSearchCV, evaluation metrics, PCA plot |
| [02 · PCA Dimensionality Reduction](./02-PCA-Dimensionality-Reduction/) | Feature reduction | PCA retaining ≥95% explained variance, variance plots, transformed datasets |

## 📈 Results from the provided notebooks

| Model / analysis | Recorded result |
|---|---:|
| KNN baseline (k=5) accuracy | **86.05%** |
| Tuned KNN accuracy | **87.15%** |
| Best KNN configuration | **k=17, Euclidean distance, uniform weights** |
| Tuned KNN ROC AUC | **0.52** |
| PCA components selected (95% variance threshold) | **8** |

> ⚠️ **Evaluation note:** The tuned KNN notebook reports ~87% accuracy but ROC AUC of just 0.52. Its recall is 1.00 for the positive class; class imbalance may explain why accuracy appears strong. Results should not be interpreted as clinical diagnostic performance. These are experimental educational notebooks, not medical tools.

## 📁 Repository layout

```text
AI-ML-Projects/
├── 01-Lung-Cancer-Prediction-KNN/
│   ├── Lung_Cancer_KNN.ipynb
│   ├── README.md
│   └── data/                      # Add your own authorized CSV
├── 02-PCA-Dimensionality-Reduction/
│   ├── PCA_Dimensionality_Reduction.ipynb
│   ├── README.md
│   ├── data/                      # Add preprocessed train/test CSVs
│   └── results/
│       ├── eda_visualizations/
│       └── outputs/
├── requirements.txt
├── .gitignore
└── README.md
```

## ⚙️ Setup

```bash
git clone https://github.com/YOUR-USERNAME/AI-ML-Projects.git
cd AI-ML-Projects
python -m venv .venv
```

Activate the virtual environment:

```powershell
# Windows PowerShell
.\.venv\Scripts\Activate.ps1
```

Install dependencies and start Jupyter:

```bash
pip install -r requirements.txt
jupyter notebook
```

Open the relevant notebook, place the required CSV dataset(s) in that project's `data/` directory, and **run the notebook with the corresponding project folder as the working directory**. The datasets are not included in this repository package.

## 🧰 Skills demonstrated

`Python` · `Data preprocessing` · `Train/test split` · `Feature scaling` · `KNN` · `Grid search` · `Cross-validation` · `Confusion matrix` · `ROC AUC` · `PCA` · `Data visualization`

## 🔐 Data and reproducibility

- Source datasets are **not included**; use datasets you have permission to share or run locally.
- Notebook paths were adjusted from local machine paths to project-relative `data/` paths.
- Notebook outputs are retained from the original uploaded files and have **not been rerun** in this package.
- Avoid committing private, identifiable, or restricted health data.

---

<div align="center">

⭐ If you find these learning projects useful, consider starring the repository!

</div>
