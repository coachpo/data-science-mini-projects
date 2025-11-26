# Congenial Computing Machine

Notebook-based machine-learning playground with three small, self-contained mini projects. Each folder ships with its dataset so you can open any notebook and run it immediately.

## What's inside
- `mini-project-1/` — UCI Bank Marketing classification; data in `bank-additional-full.csv`; multiple solution notebooks (`mini_project_1_*`).
- `mini-project-2/` — Sentiment140 tweet sentiment analysis; 10% sample TSV plus notebooks (`mini_project_2_*`, some use DistilBERT/transformers).
- `mini-project-3/` — UCI Human Activity Recognition (HAR) time-series classification; dataset split across `X_train.txt`, `X_test.txt`, `y_*`, `subject_*` with accompanying notebooks (`mini_project_3_*`).
- `requirements.txt` — Shared Python stack: numpy/pandas/scikit-learn, tensorflow/keras + tuner, torch/transformers, nltk, matplotlib/seaborn, wordcloud, emoji, contractions, pyenchant, jupyter.

## Quick start
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Work with the notebooks
```bash
jupyter notebook  # browse and run any mini_project_* notebook
# or execute headlessly
jupyter nbconvert --to notebook --execute mini-project-1/mini_project_1_my_submission.ipynb
```

## Repository layout
```
mini-project-1/        # Bank marketing classification + CSV
mini-project-2/        # Tweet sentiment notebooks + Sentiment140 sample TSV
mini-project-3/        # HAR notebooks + sensor/time-series text files
requirements.txt       # Common dependencies for all projects
.gitignore             # Keeps checkpoints, large artifacts, and envs out of git
```

## Data & outputs
- Datasets are committed for convenience; no external downloads required.
- `.gitignore` already excludes checkpoints, converted notebooks, large archives, and virtualenvs—keep new large/raw files out of git.

## Conventions
- Stay inside each `mini-project-*` folder for notebooks/data for that task.
- Use the shared `requirements.txt` to keep environments in sync.
