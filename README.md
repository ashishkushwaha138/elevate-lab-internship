# AI & ML Internship Tasks - Titanic Dataset Analysis

## Overview
This repository contains the completed tasks for the AI & ML Internship at Elevate Labs. It includes both Task 1 (Data Preprocessing) and Task 2 (Exploratory Data Analysis) performed on the Titanic dataset.

## Repository Structure
```
elevate-lab-internship/
├── task_1/                     # Task 1: Data Preprocessing
│   ├── preprocessing.py        # Data preprocessing script
│   ├── titanic_original.csv    # Original Titanic dataset
│   ├── titanic_processed.csv   # Processed dataset after cleaning
│   ├── outlier_boxplots.png    # Visualization of outliers
│   └── requirements.txt        # Python dependencies
├── task_2/                     # Task 2: Exploratory Data Analysis
│   ├── eda_titanic.py          # EDA script
│   ├── feature_inferences.txt  # Key insights from EDA
│   ├── titanic_eda_processed.csv # Processed dataset after EDA
│   └── plots/                  # Directory containing all visualizations
│       ├── histograms.png      # Histograms of numeric features
│       ├── boxplots.png        # Boxplots of numeric features
│       ├── correlation_matrix.png # Correlation matrix heatmap
│       ├── pairplot.png        # Pairplot of selected features
│       └── categorical_counts.png # Count plots of categorical features
└── README.md                   # This file
```

## Objective
Understand data using statistics and visualizations to gain insights into the Titanic dataset through two sequential tasks.

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

## Task 1: Data Preprocessing

### Analysis Performed
1. **Data Cleaning**: Handled missing values in age, embarked, and deck columns
2. **Feature Engineering**: Created new features like family size, title extraction, etc.
3. **Outlier Detection**: Identified and visualized outliers in fare and age using boxplots
4. **Data Transformation**: Normalized/scaled features where necessary
5. **Encoding**: Converted categorical variables to numerical format

### Files Created
- `preprocessing.py`: Complete preprocessing pipeline
- `titanic_processed.csv`: Cleaned and processed dataset
- `outlier_boxplots.png`: Visualization showing outliers in fare and age

## Task 2: Exploratory Data Analysis

### Analysis Performed

#### 1. Summary Statistics
Generated mean, median, standard deviation, min, max, and count for all numeric features.

#### 2. Visualizations Created
- **Histograms**: Distribution of each numeric feature
- **Boxplots**: Identification of outliers and spread of numeric features
- **Correlation Matrix**: Heatmap showing relationships between numeric features
- **Pairplot**: Pairwise relationships in the dataset (with survival coloring)
- **Count Plots**: Distribution of categorical features

#### 3. Pattern Identification
- Missing values analysis
- Survival rates by different categories (sex, class, embarkation point)
- Skewness detection in age and fare distributions

#### 4. Feature-Level Inferences
- Age distribution is right-skewed (more younger passengers)
- Fare distribution is right-skewed (few passengers paid very high fares)
- Overall survival rate: 38.38%
- Female survival rate: 74.20% vs Male survival rate: 18.89%
- Survival rate decreases with passenger class (1st > 2nd > 3rd)

## Key Learnings from Both Tasks

### From Task 1 (Preprocessing):
- Proper data cleaning is crucial for accurate analysis
- Feature engineering can reveal hidden patterns (e.g., titles correlate with survival)
- Outlier treatment affects model performance and interpretation

### From Task 2 (EDA):
- Females had significantly higher survival rate than males
- Survival rate was highest for 1st class passengers and lowest for 3rd class
- Age and fare distributions show right skewness
- Correlation analysis reveals relationships between fare, class, and survival
- Visualizations are crucial for identifying patterns, trends, and anomalies in data

## How to Run

### Task 1: Data Preprocessing
```bash
# Navigate to task_1 directory
cd task_1

# Ensure you have Python 3.x installed
# Install required packages:
pip install -r requirements.txt

# Run the preprocessing script:
python preprocessing.py

# Output: titanic_processed.csv and outlier_boxplots.png
```

### Task 2: Exploratory Data Analysis
```bash
# Navigate to task_2 directory
cd task_2

# Ensure you have Python 3.x installed
# Install required packages (if not already installed):
pip install pandas numpy matplotlib seaborn

# Run the EDA script:
python eda_titanic.py

# Output: Updated visualizations in plots/ directory and feature_inferences.txt
```

## Submission
After completing both tasks, the GitHub repository link should be submitted via the provided submission link.

---
*This repository contains the completed work for Tasks 1 and 2 of the AI & ML Internship at Elevate Labs.*