# Homework 02 — Regression

- Task: https://github.com/DataTalksClub/machine-learning-zoomcamp/blob/main/cohorts/2026/homework/02-regression/homework.md
- Local task: [homework.md](homework.md)
- Executed solution: [homework.ipynb](homework.ipynb)
- Submission: https://courses.datatalks.club/ml-zoomcamp-2026/homework/hw02

## Reproduce

From the repository root, activate the environment and open the notebook:

```bash
source .venv/bin/activate
pip install numpy pandas matplotlib jupyter certifi
jupyter notebook 02-regression/homework.ipynb
```

Run all cells in order. The notebook downloads and caches the 2026 dataset if
needed; the CSV is excluded from Git. It includes target EDA, the prescribed
splits, linear regression from scratch, and all six calculations.

## Answers

| Question | Answer | Calculation |
|---|---|---|
| 1. Missing values | `horsepower` | 877 missing values |
| 2. Median horsepower | **254** | Median before imputation |
| 3. Filling NAs | **With mean** | Validation RMSE: 2.202 vs. 2.205 with zero |
| 4. Best regularization | **0** | Validation RMSE: 2.2053 |
| 5. RMSE standard deviation | **0.029** | `np.std` across seeds 0–9: 0.028781 |
| 6. Evaluation on test | **2.236** | Seed 9, train + validation, `r=0.001`: 2.235828 |
