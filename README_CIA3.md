# Forest-Fire Risk Prediction using Ensemble Machine Learning

**Student:** Aditi Ahuja  
**Course:** Machine Learning (MCA 521-4)  
**Assessment:** CIA 3 – ML for Social Good Challenge  
**Mission:** Earth – Environment

## 1\. Project Description

This project uses ensemble machine learning to predict forest-fire risk from environmental and fire-weather data. The project compares Logistic Regression, Random Forest, XGBoost and a Stacking Ensemble, followed by SHAP-based explainability and a live synthetic prediction.

## 2\. Dataset

**UCI Forest Fires Dataset**

Source: https://archive.ics.uci.edu/dataset/162/forest%2Bfires  
DOI: 10.24432/C5D88D

The dataset contains 517 observations from the Montesinho region of Portugal. The `area` variable is converted into a binary target:

* `0` = no fire (`area = 0`)
* `1` = fire (`area > 0`)

## 3\. Files

```text
Forest-Fire-Risk-Prediction/
├── ForestFire\_RiskPrediction.ipynb
├── README.md
```

The complete analysis, preprocessing, modelling, evaluation, SHAP explainability and live prediction are contained in the notebook.

## 4\. Requirements

Python packages used:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
shap
jupyter
```

Install with:

```bash
pip install -r requirements.txt
```



## 5\. Reproducibility

The notebook uses:

* A stratified train/test split.
* Cross-validation during model development.
* Pipeline-based preprocessing to reduce data leakage.
* An untouched test set for final model comparison.
* Fixed random states where applicable.

## 8\. Models

* Logistic Regression — baseline
* Random Forest — bagging
* XGBoost — boosting
* Stacking Ensemble — Random Forest + XGBoost → Logistic Regression

The final model comparison and detailed interpretation are provided in the Word report.

## 9\. Explainability

SHAP is used for:

* **Global explanation** — overall feature importance.
* **Local explanation** — explanation of an individual prediction.

The SHAP outputs are presented in the Word report.



