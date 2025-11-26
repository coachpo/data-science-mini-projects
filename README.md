# Congenial Computing Machine

Lightweight collection of three data-science mini projects, each self-contained with its notebook and small sample datasets. Use this repo to review or rerun experiments without hunting for external assets.

## Structure
- `mini-project-1/` – Bank Marketing classification (UCI Bank Marketing); data in `bank-additional-full.csv`, notebooks `mini_project_1_*`.
- `mini-project-2/` – Tweet sentiment analysis (Sentiment140 10% sample); data in `Sentiment140.tenPercent.sample.tweets.tsv`, notebooks `mini_project_2_*`.
- `mini-project-3/` – Human activity recognition (UCI HAR); data split across `X_train.txt`, `X_test.txt`, `y_train.txt`, `y_test.txt`, `subject_*`, notebooks `mini_project_3_*`.
- `requirements.txt` – Shared Python dependencies for all notebooks.

## Setup
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Running notebooks
```bash
jupyter notebook  # then open the notebook you want
# or
jupyter nbconvert --to notebook --execute mini-project-1/mini_project_1_my_submission.ipynb
```

## Data notes
- Datasets are already checked into the repo for convenience; they are small but still excluded from future commits via `.gitignore` patterns for other large/raw data you might add.
- Keep new outputs (checkpoints, converted notebooks, large logs) out of git; the `.gitignore` is configured accordingly.

## Repo conventions
- Default branch: `main`.
- Keep notebooks and data per project under their respective `mini-project-*` folder.
- Use `pip install -r requirements.txt` to stay aligned across projects.
