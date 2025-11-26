# Predicting Anime Success — Regression Project

This repository contains a Jupyter Notebook that demonstrates a hands-on regression workflow to predict an anime's ranking using features such as score, popularity, members, favorited counts, and genre one-hot encodings.

## Project summary
- Notebook: `Predicting Anime Success, A Hands-On Data Regression Project.ipynb`
- Dataset: `anime_entries.csv` (from Kaggle — https://www.kaggle.com/datasets/hamzaashfaque1999/myanimelist-scraped-data)
- Goal: Build and compare regression models (XGBoost, AdaBoost, Linear Regression) to predict the `ranked` target and evaluate using MAE, RMSE and R².

## Key steps performed in the notebook
1. Data loading and formatting (parsing `airing_date`, converting list-like columns).
2. Missing-value handling (drop high-missing columns, regression imputation for `score` and `ranked`).
3. Feature engineering (genre one-hot encoding via `MultiLabelBinarizer`, binning `airing_date`).
4. Normalization (z-score via `StandardScaler()` for `members` and `scored_by`).
5. Exploratory Data Analysis (boxplots, histograms, scatterplots, heatmaps, time-series plots).
6. Model training and evaluation: XGBoost, AdaBoost, and Multilinear Regression.

## Dependencies
Recommended Python environment with these packages installed (example):

- python >= 3.8
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost (optional, used for XGBoost model)

You can install them via pip, for example:

```powershell
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

## How to run
1. Open the notebook in Jupyter or JupyterLab:

```powershell
jupyter lab "d:\your\directory\path\Predicting Anime Success, A Hands-On Data Regression Project.ipynb"
```

2. Make sure `anime_entries.csv` is in the same directory as the notebook.
3. Execute the cells in order. 