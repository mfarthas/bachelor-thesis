# Bachelor Thesis Project
## Evaluation of Network Intrusion Detection Using Machine Learning

## Overview
This project is the implementation component of a bachelor thesis focused on the application and evaluation of machine learning techniques for network intrusion detection. The primary objective is to analyze how different data preprocessing strategies and feature representations affect the performance of supervised learning models on intrusion detection datasets.

All experiments are conducted using Python and Jupyter Notebooks.

## Problem Statement
Traditional rule-based intrusion detection systems struggle to scale and adapt to evolving network threats. Machine learning offers a data-driven alternative, but its effectiveness depends heavily on data quality, preprocessing decisions, and feature engineering choices.

This project investigates:
- The impact of raw versus processed network traffic features
- The trade-offs between minimal and extensive feature engineering
- The robustness of models across synthetic and real-world datasets

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
The project uses benchmark and real intrusion detection datasets.

A curated subset of the CICIDS dataset is employed, selected and preprocessed to support controlled experimentation and reproducibility. The dataset is stored locally in multiple derived forms representing different feature engineering strategies.

## Methodology
1. Data preprocessing
   - Cleaning and normalization
   - Feature selection and transformation
   - Dataset partitioning

2. Feature engineering strategies
   - Raw feature baseline
   - Reduced feature representation
   - Over-engineered feature set

3. Model training and evaluation
   - Supervised learning models
   - Consistent evaluation metrics
   - Comparative analysis of results

## Key Findings
- Feature engineering significantly affects model performance.
- Over-engineering does not consistently improve results.
- Data preprocessing quality is as important as model choice.

## Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## How to Run
1. Ensure Python 3.x is installed.
2. Install dependencies:
```
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```
3. Start Jupyter:
```
jupyter notebook
```
4. Run notebooks starting with RAW.ipynb or UCIdata.ipynb.

## Skills Demonstrated
- Applied machine learning
- Experimental design
- Feature engineering
- Data analysis
- Reproducible research
