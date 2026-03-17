# Evaluating CTGAN-generated Synthetic Firewall Logs through Statistical and Structural Analysis

## Overview

Implementation component of a bachelor thesis on ML-based network intrusion detection. The main question: how much do preprocessing decisions and feature representations actually affect model performance?

All experiments run in Python and Jupyter Notebooks.

## Problem Statement

Rule-based IDS doesn't scale and struggles with novel attack patterns. ML handles this better in principle, but performance depends heavily on the data pipeline, not just the model.

This project examines three things:
- Raw versus processed network traffic features as model input
- Whether heavier feature engineering pays off
- Model robustness across synthetic and real-world data

## Project Structure
```
bachelor-thesis/
├── Real Data/
│   ├── cicids_cleaned.csv
│   ├── RAW_REAL.csv
│   ├── OverEngineeredREAL.csv
│   ├── BackAndForthREAL.csv
│   ├── log2.csv
│   └── analysis notebooks
├── Jupyter notebooks/
│   ├── RAW.ipynb
│   ├── Reduced.ipynb
│   ├── OverEngineered.ipynb
│   ├── RawQualityTest.ipynb
│   ├── UCIdata.ipynb
│   └── supporting analysis notebooks
└── Supporting files and checkpoints
```

## Datasets

A curated CICIDS subset, stored in multiple derived forms — each representing a different preprocessing strategy.

## Methodology

Preprocessing covers cleaning, normalization, feature selection, and partitioning. Three feature engineering strategies are compared: a raw baseline, a reduced feature set, and an over-engineered variant. All models are evaluated on the same metrics to keep comparisons clean.

## Findings

More feature engineering didn't help reliably. The over-engineered feature set performed worse or comparably to simpler representations in most experiments. Preprocessing quality ended up mattering about as much as model choice — sometimes more.

## Technologies

Python, Jupyter Notebook, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## How to Run
```
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook
```

Start with `RAW.ipynb` or `UCIdata.ipynb`.
