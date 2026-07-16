# Chronic Kidney Disease Prediction Using Machine Learning

An academic machine-learning project for predicting chronic kidney disease (CKD) using three supervised classification approaches: LASSO logistic regression, decision tree, and neural network.

## Project overview

This repository contains the analytical report, reproducible Jupyter notebook, aggregate validation tables, and visualization outputs for the Data Mining and Machine Learning final examination. The individual-level health dataset and row-level predictions are intentionally not distributed in this public repository.

**Author:** Mohammad Maliki Rafli  
**Program:** Master of Public Health, Universitas Airlangga

## Methods

- Missing-data handling through model pipelines
- Stratified training and internal-validation split
- Hyperparameter tuning with stratified cross-validation
- LASSO logistic regression
- Decision tree classification
- Multilayer perceptron neural network
- Discrimination, calibration, and classification-performance assessment
- Bootstrap confidence intervals and feature-importance analysis

## Main validation results

| Model | Accuracy | Sensitivity | Specificity | F1 score | AUC | Brier score |
|---|---:|---:|---:|---:|---:|---:|
| LASSO logistic regression | 1.00 | 1.00 | 1.00 | 1.000 | 1.000 | 0.0016 |
| Decision tree | 0.99 | 1.00 | 0.974 | 0.992 | 0.998 | 0.0124 |
| Neural network | 0.98 | 0.968 | 1.00 | 0.984 | 1.000 | 0.0665 |

These results describe internal validation on this dataset and should not be interpreted as evidence of external clinical validity. Independent external validation is required before any clinical application.

## Repository structure

```text
.
|-- 01_Laporan/   # Final analytical report (PDF)
|-- 02_Script/    # Reproducible Jupyter notebook
|-- 03_Data/      # Local dataset directory (not tracked)
|-- 04_Output/    # Metrics, predictions, tables, and figures
|-- README.md
|-- requirements.txt
`-- .gitignore
```

## Reproducing the analysis

1. Clone the repository.
2. Create and activate a Python virtual environment.
3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Create the directory `03_Data/` and place the required dataset at `03_Data/data_uas_kidney_disease.csv`.
5. Open the notebook in `02_Script/` and run all cells from top to bottom.

## Notes

- The repository is intended for academic and educational use.
- The individual-level health dataset is excluded to protect data privacy and prevent unauthorized redistribution.
- Row-level validation predictions are also excluded; only aggregate performance results are published.
- Model estimates may be optimistic because they are based on internal validation.
- The included report provides the complete methodological explanation and interpretation.
