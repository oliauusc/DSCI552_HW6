# DSCI 552 — Homework 6

Machine learning homework on tree-based methods (random forests, XGBoost model
trees) with missing-data imputation and SMOTE on the APS Failure at Scania
Trucks dataset, plus written answers to ISLR exercises 6.6.3, 6.6.5, 8.4.5,
and 9.7.3.

## How to run

1. Install dependencies: `pip install -r requirements.txt`
   (also `pip install jupyterlab ipykernel` if you do not have Jupyter yet)
2. Launch Jupyter from the repository root: `jupyter lab` (or `jupyter notebook`)
3. Open `notebook/Liau_Olivia_HW6.ipynb`
4. Run **Kernel → Restart Kernel and Run All Cells** (Cell → Run All)
5. The notebook runs from a fresh kernel with no errors; relative paths assume
   it is executed in place inside this repository layout.

## Data

`data/aps_failure/` contains the APS Failure at Scania Trucks dataset from the
UCI Machine Learning Repository
(https://archive.ics.uci.edu/ml/datasets/APS+Failure+at+Scania+Trucks):
the training set (60,000 rows), the test set (16,000 rows), and the dataset
description with the challenge cost metric. The data files are committed to
the repository on purpose so the notebook runs as-is.

## Expected runtime

The full Run All takes about **4 minutes** on the machine used to prepare this
submission (im on m4 Apple Silicon laptop). Random forests and the cross-validated XGBoost/SMOTE sweeps dominate; per-cell elapsed times are printed in the notebook.

## Contents

- `notebook/Liau_Olivia_HW6.ipynb` — the full homework (handout questions
  quoted verbatim, followed by approach, code, and written answers)
- `notebook/figures/` — screenshots of the ISLR exercise statements embedded
  in the notebook
- `requirements.txt` — pinned library versions
