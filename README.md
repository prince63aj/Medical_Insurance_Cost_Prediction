# Medical Insurance Cost Prediction Using Machine Learning

## Project Overview

Medical insurance charges vary from person to person depending on factors such as age, BMI, smoking habits, gender, number of children and residential region.

The aim of this project is to analyse these factors and develop a Machine Learning model that predicts an individual's medical insurance expenses using regression algorithms.

This project uses Python for data analysis, visualization, data preprocessing and model development.

## Objectives

- Understand the factors that influence medical insurance charges.
- Perform Exploratory Data Analysis (EDA) to identify patterns and relationships.
- Clean and preprocess the dataset.
- Apply feature engineering and feature selection.
- Build and compare different regression models.
- Improve model performance using hyperparameter tuning.
- Evaluate the final model using appropriate regression metrics.

## Dataset Information

**Dataset Name:** Medical Cost Personal Dataset

**Source:** Kaggle

**Dataset Link:** https://www.kaggle.com/datasets/mirichoi0218/insurance

**Dataset Details:**
- Total Records: 1,338
- Total Columns: 7
- File Format: CSV
- Target Variable: `charges`

### Dataset Attributes

| Column | Description |
|---|---|
| age | Age of the individual |
| sex | Gender of the individual |
| bmi | Body Mass Index |
| children | Number of dependents |
| smoker | Smoking status (yes/no) |
| region | Residential region |
| charges | Individual medical insurance expenses |

## Technologies and Libraries Used

- Python
- Pandas – Data manipulation and analysis
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Scikit-learn – Machine Learning and model evaluation

## Project Workflow

### 1. Data Understanding
- Loading the dataset.
- Understanding dataset structure and attributes.
- Checking data types and statistical summaries.

### 2. Exploratory Data Analysis (EDA)
- Distribution of medical insurance charges.
- Age and insurance charges relationship.
- BMI and insurance charges relationship.
- Impact of smoking habits on insurance expenses.
- Comparison of charges across different regions and demographic groups.
- Correlation analysis.

### 3. Data Cleaning and Preprocessing
- Handling missing values.
- Removing duplicate records.
- Checking inconsistent records.
- Detecting and handling outliers.
- Encoding categorical variables.
- Feature scaling.

### 4. Feature Engineering
- Creating age groups.
- Creating BMI categories.
- Creating smoking-related interaction features.
- Exploring relationships between smoking, BMI and age.

### 5. Machine Learning Models

The following regression algorithms are implemented:

1. Linear Regression
2. Ridge Regression
3. Random Forest Regressor
4. Gradient Boosting Regressor

### 6. Hyperparameter Tuning

GridSearchCV with 5-fold cross-validation is used to tune the selected models and improve their performance.

Linear Regression is retained as a baseline model without hyperparameter tuning.

### 7. Model Evaluation

The models are evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

Model performance is compared before and after hyperparameter tuning.

### 8. Final Model Analysis

- Testing the selected model on the untouched test dataset.
- Comparing actual and predicted insurance charges.
- Analysing residuals.
- Identifying important features using permutation importance.
- Documenting findings, limitations and conclusions.

## Project Structure

```text
Medical-Insurance-Cost-Prediction/
│
├── Analysis.ipynb
│
├── insurance.csv
│
└── README.md
```

## Installation and Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/prince63aj/Medical_Insurance_Cost_Prediction
```

### Step 2: Navigate to the Project Folder

```bash
cd Medical-Insurance-Cost-Prediction
```

### Step 3: Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Step 4: Open the Notebook

Open the project folder in Visual Studio Code.

Open `Analysis.ipynb` and select your Python environment.

### Step 5: Run the Notebook

Execute all notebook cells in order to perform the complete analysis and train the regression models.

Make sure `insurance.csv` is present in the same directory as the notebook.

## Key Findings

The analysis explores the influence of different demographic and lifestyle factors on medical insurance expenses.

Some important patterns investigated include:

- Smoking status has a strong relationship with insurance charges.
- Insurance expenses generally increase with age.
- BMI can influence insurance costs, particularly among smokers.
- Regional and gender-based differences are also examined.

## Limitations

- The dataset contains only 1,338 records.
- The available attributes are limited to the information provided in the dataset.
- The model cannot account for every individual medical condition or insurance policy detail.
- Predictions are estimates and may differ from actual insurance premiums.

## Conclusion

This project demonstrates how Machine Learning regression algorithms can be used in Healthcare Analytics to estimate medical insurance expenses.

Through Exploratory Data Analysis, preprocessing, feature engineering and model evaluation, the project identifies important factors associated with insurance charges and compares different regression algorithms.

The project also provides practical experience in applying Python and Machine Learning techniques to a real-world prediction problem.

---

**Project Domain:** Healthcare Analytics

**Project Type:** Machine Learning – Regression

**Programming Language:** Python

**Development Environment:** Visual Studio Code
