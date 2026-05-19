# Stroke Prediction — Binary Classification

Predicts stroke risk from patient health and lifestyle data using multiple classical ML algorithms. Models are compared across accuracy, precision, recall, and F1-score.

## Task

Given a patient's health profile, predict whether they are at risk of having a stroke (binary: 0 = No stroke, 1 = Stroke).

## Dataset Features

| Feature | Description |
|---------|-------------|
| Age | Patient age |
| Hypertension | 0 or 1 |
| Heart Disease | 0 or 1 |
| Marital Status | Ever married |
| Work Type | Private / Self-employed / Govt / Children / Never worked |
| Residence Type | Urban / Rural |
| Avg Glucose Level | Blood glucose (mg/dL) |
| BMI | Body mass index |
| Smoking Status | Formerly smoked / Never / Smokes / Unknown |

## Models Compared

| Model | Notes |
|-------|-------|
| Logistic Regression | Baseline linear classifier |
| Random Forest | Ensemble, handles class imbalance well |
| Support Vector Machine | RBF kernel |
| K-Nearest Neighbors | Distance-based |
| Decision Tree | Interpretable, prone to overfitting |

Evaluation metrics: **Accuracy · Precision · Recall · F1-Score**

## Methodology

- **Preprocessing**: Missing value imputation (BMI), categorical encoding, feature scaling
- **Split**: Stratified train/test split to preserve class imbalance ratio
- **Imbalance handling**: Class weighting / SMOTE where applicable
- **Visualization**: Correlation heatmaps, feature importance, ROC curves, confusion matrices

## Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)

`scikit-learn` · `pandas` · `numpy` · `matplotlib` · `seaborn`

## Project Structure

```
Stroke-Prediction-Binary-Classification/
├── Stroke_Prediction_Binary_Classification.ipynb   # Full pipeline
└── README.md
```

## Getting Started

```bash
git clone https://github.com/kaltisami/Stroke-Prediction-Binary-Classification.git
cd Stroke-Prediction-Binary-Classification
pip install scikit-learn pandas numpy matplotlib seaborn
```

Open the notebook in Jupyter or Google Colab and run all cells.

## Related Projects

- [chest-xray-ai-diagnosis](https://github.com/kaltisami/chest-xray-ai-diagnosis) — production-grade chest X-ray analysis platform
- [Parkinson-s-Disease-CT-Brain-Images-Classification](https://github.com/kaltisami/Parkinson-s-Disease-CT-Brain-Images-Classification) — CT brain image classification with DenseNet121

## License

MIT
