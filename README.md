# Depression Risk Analysis

This repository contains my local-environment adaptation of the Kaggle notebook originally authored by **moridata**:  
[Key Factors in Depression Risk](https://www.kaggle.com/code/moridata/key-factors-in-depression-risk). All code has been updated to run outside of Kaggle, using data stored here.

---

## Author

**Your Name**  
GitHub: (https://github.com/MoriData)  
Email: mori.py.data@gmail.com


---

## Problem Explanation

Depression affects hundreds of millions of adults worldwide and often goes undetected until symptoms become severe. In non-clinical, community settings, it’s challenging to know which individuals are at highest risk—especially when relying solely on basic demographics. By analyzing self-reported survey data (e.g., stress levels, satisfaction, suicidal thoughts, lifestyle measures) and applying machine learning, we aim to identify a small set of high-impact questions that can quickly flag adults most likely to be experiencing depression. Early, data-driven screening like this can guide timely interventions and reduce the overall burden of mental illness.

## Summary of Findings

We analyzed survey data from 2,556 adult respondents (ages 18–60) to determine which demographic, psychosocial, and lifestyle features most strongly predict self-reported depression. We trained a CatBoost model—accounting for class imbalance through weighted loss—and achieved 95.7 % accuracy on a held-out test set. The model’s top predictors include Age, Suicidal Thoughts, Combined Work/Academic Pressure, and Combined Job/Study Satisfaction.


## Project Overview

The goal of this project is to identify which demographic and behavioral factors most strongly predict depression risk. Starting from the Kaggle notebook “Key Factors in Depression Risk,” I have:

1. Downloaded and stored the original CSV locally.  
2. Modified all data-loading paths to reference `data/` instead of Kaggle’s mounted directories.  
3. Removed any Kaggle-specific commands.  
4. Added (optional) enhancements—see the **Extensions** section below.

The notebook performs:

- Exploratory Data Analysis (EDA)  
- Preprocessing (handling missing values, encoding categorical variables)  
- Model training (e.g., Logistic Regression, Random Forest)  
- Feature importance ranking  
- Interpretation of results

---


- **`data/`**  
  Contains the original dataset file (`depression_data.csv`). If you want to refresh or replace the data, download the CSV from:
https://www.kaggle.com/datasets/sumansharmadataworld/depression-surveydataset-for-analysis

