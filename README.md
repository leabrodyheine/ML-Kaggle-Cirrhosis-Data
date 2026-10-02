# Cirrhosis Outcome Classification

A completed machine-learning coursework project for the Kaggle *Multi-Class Prediction of Cirrhosis Outcomes* dataset. The analysis explores clinical features, compares missing-value strategies, addresses class imbalance, trains several classifier families, and produces competition submissions.

## Highlights

- Exploratory analysis of numerical and categorical clinical variables
- Median/mode, nearest-neighbour, and model-based imputation experiments
- Standardization, one-hot encoding, and feature engineering
- SMOTE and random undersampling for imbalanced outcomes
- Logistic regression, support-vector machine, random forest, and XGBoost models
- Hyperparameter tuning and a Random Forest/XGBoost ensemble
- Feature-importance analysis and submission generation

The imputation experiment found that nearest-neighbour and model-based imputation produced the strongest downstream Kaggle results, with log loss of 0.44962 and 0.44971 respectively in the recorded runs.

## Repository contents

- `ID5059_P2_Final.ipynb` is the complete analysis and modeling workflow.
- `Imputation Method.ipynb` isolates the imputation comparison.
- `train.csv`, `test.csv`, and `sample_submission.csv` are the competition data files used by the notebooks.
- The remaining CSV files are saved model predictions and submissions.
- `impuation models- kaggle results.pdf` records the competition results.

## Run the analysis

Create an environment with the pinned dependencies and open the main notebook:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter lab ID5059_P2_Final.ipynb
```

The dependency snapshot targets Python 3.11-era packages and includes Jupyter, pandas, scikit-learn, imbalanced-learn, XGBoost, TensorFlow, and visualization libraries.

## Project status

This repository contains the completed analysis, saved outputs, and submitted predictions. It is preserved as a reproducible academic project rather than an actively maintained clinical tool.
