# Elevate Lab Internship - AIML Task 1: Data Cleaning & Preprocessing

## Overview
This repository contains the solution for Task 1: Data Cleaning & Preprocessing from the AI & ML Internship at Elevate Labs.

## Objective
Learn how to clean and prepare raw data for Machine Learning.

## Tools Used
- Python 3.12.3
- Pandas
- NumPy
- Matplotlib/Seaborn
- Scikit-learn

## Files in this Repository
- `preprocessing.py`: Python script performing all preprocessing steps
- `titanic_original.csv`: Original Titanic dataset (downloaded from seaborn)
- `titanic_processed.csv`: Cleaned and preprocessed dataset after all steps
- `outlier_boxplots.png`: Visualization showing boxplots before and after outlier removal (for fare column)
- `requirements.txt`: Python dependencies required to run the script
- `README.md`: This file

## Steps Performed

1. **Imported the dataset and explored basic info** (nulls, data types)
2. **Handled missing values** using mean/median/imputation:
   - Numerical columns (age): filled with median (28.0)
   - Categorical columns (embarked, deck, embark_town): filled with mode
3. **Converted categorical features into numerical** using one-hot encoding (pd.get_dummies with drop_first=True)
4. **Normalized/standardized the numerical features** using StandardScaler (zero mean, unit variance)
5. **Visualized outliers using boxplots and removed them** using IQR method (Q1 - 1.5*IQR, Q3 + 1.5*IQR)

## Key Learnings Demonstrated
- Different types of missing data (MCAR, MAR, MNAR)
- Techniques for handling categorical variables (Label Encoding vs One-Hot Encoding)
- Difference between normalization (Min-Max scaling) and standardization (Z-score normalization)
- Methods to detect outliers (IQR method, boxplots, Z-score)
- Importance of preprocessing in ML (improves model accuracy, reduces training time, handles missing data)
- How preprocessing can affect model accuracy (both positively and negatively)

## Results
- Original dataset shape: (891, 15)
- After processing and outlier removal: (598, 24)
- Removed 293 outlier rows based on IQR method across numerical features
- Features after one-hot encoding: 24 columns (including encoded categorical variables)
- Numerical features standardized: survived, pclass, age, sibsp, parch, fare

## How to Run
1. Ensure you have Python 3.x installed
2. Install required packages: `pip install -r requirements.txt`
3. Run the script: `python3 preprocessing.py`
4. The processed dataset will be saved as `titanic_processed.csv`

## Internship Details
- **Position:** AIML Intern
- **Company:** Elevate Labs
- **Duration:** 45-day remote internship
- **Start Date:** September 28, 2026
- **Benefits:** Completion certificate and Letter of Recommendation (LOR)
- **Contact:** hr@elevate-labs.info

## Submission
This repository fulfills the Task 1 submission requirements for the AI & ML Internship at Elevate Labs.
All work is original and completed using free, open-source tools as per internship guidelines.