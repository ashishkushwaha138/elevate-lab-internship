# Exploratory Data Analysis (EDA) - Titanic Dataset

## Overview
This repository contains the exploratory data analysis of the Titanic dataset as part of the AI & ML Internship Task 2. The analysis includes generating summary statistics, creating visualizations (histograms, boxplots, correlation matrix, pairplot), identifying patterns and trends, and making feature-level inferences.

## Objective
Understand data using statistics and visualizations to gain insights into the Titanic dataset.

## Tools Used
- Python 3.x
- Pandas - Data manipulation and analysis
- NumPy - Numerical operations
- Matplotlib - Data visualization
- Seaborn - Statistical data visualization

## Dataset
The Titanic dataset contains information about passengers aboard the Titanic, including whether they survived or not. Key features include:
- survived: Survival (0 = No, 1 = Yes)
- pclass: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)
- sex: Sex of the passenger
- age: Age in years
- sibsp: Number of siblings/spouses aboard
- parch: Number of parents/children aboard
- fare: Passenger fare
- embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Analysis Performed

### 1. Summary Statistics
Generated mean, median, standard deviation, min, max, and count for all numeric features.

### 2. Visualizations Created
- **Histograms**: Distribution of each numeric feature
- **Boxplots**: Identification of outliers and spread of numeric features
- **Correlation Matrix**: Heatmap showing relationships between numeric features
- **Pairplot**: Pairwise relationships in the dataset (with survival coloring)
- **Count Plots**: Distribution of categorical features

### 3. Pattern Identification
- Missing values analysis
- Survival rates by different categories (sex, class, embarkation point)
- Skewness detection in age and fare distributions

### 4. Feature-Level Inferences
- Age distribution is right-skewed (more younger passengers)
- Fare distribution is right-skewed (few passengers paid very high fares)
- Overall survival rate: 38.38%
- Female survival rate: 74.20% vs Male survival rate: 18.89%
- Survival rate decreases with passenger class (1st > 2nd > 3rd)

## Files in Repository
- `eda_titanic.py`: Python script performing the EDA
- `titanic_original.csv`: Original Titanic dataset
- `titanic_eda_processed.csv`: Processed dataset (after EDA)
- `feature_inferences.txt`: Text file containing key inferences from the analysis
- `plots/`: Directory containing all visualizations:
  - `histograms.png`: Histograms of numeric features
  - `boxplots.png`: Boxplots of numeric features
  - `correlation_matrix.png`: Correlation matrix heatmap
  - `pairplot.png`: Pairplot of selected features
  - `categorical_counts.png`: Count plots of categorical features

## How to Run
1. Ensure you have Python 3.x installed
2. Install required packages:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Run the EDA script:
   ```bash
   python eda_titanic.py
   ```
4. Check the `plots/` directory for visualizations and `feature_inferences.txt` for key insights

## Key Learnings
- Females had significantly higher survival rate than males
- Survival rate was highest for 1st class passengers and lowest for 3rd class
- Age and fare distributions show right skewness
- Correlation analysis reveals relationships between fare, class, and survival
- Visualizations are crucial for identifying patterns, trends, and anomalies in data

## Submission
After completing the task, the GitHub repository link should be submitted via the provided submission link.

---
*This analysis was performed as part of Task 2: Exploratory Data Analysis (EDA) for the AI & ML Internship.*