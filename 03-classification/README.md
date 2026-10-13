# Homework 03 — Classification

- Task: https://github.com/DataTalksClub/machine-learning-zoomcamp/blob/main/cohorts/2026/homework/03-classification/homework.md
- Local task: [homework.md](homework.md)
- Executed solution: [homework.ipynb](homework.ipynb)
- Submission: https://courses.datatalks.club/ml-zoomcamp-2026/homework/hw03

## Reproduce

From the repository root, activate the environment and open the notebook:

```bash
source .venv/bin/activate
pip install numpy pandas scikit-learn jupyter certifi
jupyter notebook 03-classification/homework.ipynb
```

Run all cells in order. The notebook downloads and caches the 2026 dataset if
needed; the CSV is excluded from Git. It covers missing-value imputation, the
prescribed splits, mutual information, logistic regression, feature
elimination, and regularization tuning.

## Answers

| Question | Answer | Calculation |
|---|---|---|
| 1. Mode for industry | **`technology`** | 1,173 rows |
| 2. Biggest correlation | **`interaction_count` and `lead_score`** | 0.916 |
| 3. Biggest MI | **`lead_source`** | 0.03 (training set) |
| 4. Accuracy | **0.65** | Validation accuracy 0.645 |
| 5. Feature selection | **`number_of_courses_viewed`** | Difference 0.002 (`lead_source` 0.003, `interaction_count` 0.044) |
| 6. Parameter tuning | **0.001** | Validation accuracy 0.645 |
