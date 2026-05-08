# Report-A_Replication

This repository contains the code and data used for my Data Science Research Project Part A progress report.

The project includes two parts:

1. a reproduction study based on Ryan et al. (2025), focusing on COVID-19 protective behaviours in Australia;
2. a preliminary exploratory analysis for my own project, focusing on self-isolation willingness and perceived feasibility in the China sample.

## Repository structure

```text
Report-A_Replication/
│
├── code/
│   ├── 01_clean_data.ipynb
│   ├── 02_preprocess_data.ipynb
│   ├── 03_split_data.ipynb
│   ├── 04_prepare_model1.ipynb
│   ├── 05_prepare_model2.ipynb
│   ├── 06_logistic_regression.ipynb
│   ├── 07_random_forest.ipynb
│   ├── 08_xgboost.ipynb
│   ├── 09_classification_tree.ipynb
│   ├── 10_feature_importance.ipynb
│   └── 11_china_comparison.ipynb
│
├── data/
│   └── raw.zip
│
├── results/
│   ├── figures/
│   └── xgb_feature_importance_plots/
│
└── README.md
```

## Code workflow

The notebooks should be run in numerical order.

The workflow includes:

- cleaning the raw Australia survey data;
- preprocessing the Australia survey data and Australian policy data;
- creating train-test splits;
- preparing model input files for face mask behaviour and general protective behaviour;
- fitting and evaluating logistic regression, classification tree, random forest, and XGBoost models;
- generating XGBoost feature importance plots;
- conducting a preliminary China and Australia comparison of self-isolation willingness and perceived feasibility.

## Data

The `data/` folder contains `raw.zip`. After extracting this file, the `raw/` folder contains three raw data files:

- `australia.csv`: the Australia sample from the Imperial College London YouGov COVID-19 Behaviour Tracker dataset;
- `china.csv`: the China sample from the Imperial College London YouGov COVID-19 Behaviour Tracker dataset;
- `OxCGRT_AUS_latest.csv`: Australian policy data from the Oxford COVID-19 Government Response Tracker.

## Results

The `results/` folder contains the final figures used in the progress report. The `figures/` folder contains the China and Australia heatmap comparing self-isolation willingness and perceived feasibility, and the `xgb_feature_importance_plots/` folder contains the XGBoost feature importance plots.

## Acknowledgement

The code workflow and modelling logic in this repository were developed with reference to Ryan et al. (2025). Part of the code used in the data cleaning and preprocessing notebooks was directly taken from the code used in Ryan et al. (2025).
