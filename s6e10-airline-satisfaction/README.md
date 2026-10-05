# Playground S6E10: Predicting Airline Satisfaction

[Kaggle competition](https://www.kaggle.com/competitions/playground-series-s6e10)

## Task

Predict whether an airline passenger was satisfied, from service ratings, flight details and passenger attributes. Binary classification, evaluated on **ROC AUC** of the predicted probabilities.

- Train: ~700k rows. Test: ~300k rows (synthetic data generated from a real-world dataset).
- Submission format: `id,satisfaction` with a probability per row.
- Final submission deadline: 31 Oct 2026.

## Layout

```
data/raw/        original competition files (never edited, git-ignored)
data/interim/    cleaned copies (git-ignored)
data/processed/  model-ready feature tables (git-ignored)
notebooks/       numbered exploration notebooks
src/             config, features, validation, train and predict scripts
models/          saved models, one per experiment ID (git-ignored)
oof/             out-of-fold and test predictions per experiment (git-ignored)
submissions/     submission CSVs named by experiment ID (git-ignored)
results/         experiments.csv: one row per experiment
reports/figures/ plots
```

## Method

Experiments are logged in `results/experiments.csv` with an ID (`exp001`, ...) that also names the model, prediction and submission files, so any leaderboard score traces back to the code that produced it.

## Reproducing

Place the competition files in `data/raw/`, then `pip install -r requirements.txt`. Scripts will be documented here as they are written.

## Results

To be filled in as experiments are run.
