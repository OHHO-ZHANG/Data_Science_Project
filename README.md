# Data_Science_Project
This study applies data science to analyze employee attrition. After removing variables with high missing rates and data leakage risks, exploratory analysis confirms that low income, heavy overtime, and lack of promotion significantly increase attrition risk.

# Datasets

* **HR_Attrition Data.csv** – **Training/Master Dataset**. Contains detailed information on 1470 employees, covering demographic indicators, job roles, satisfaction ratings, and attrition status. This data forms the basis for building the predictive model.
* **HR_New_data.csv** – **New dataset/test set**. Used to validate model performance or simulate real-world scenarios for assessing the risk of new employee turnover.

# What the Notebooks does
## 1.Data Cleaning & Preprocessing
### I. Handling Missing Data
We identified variables with over 80% missing values (e.g., Attrition Date) and removed them to ensure data quality.

### II. Dataset Integration
Multiple data sources were merged into a unified dataframe, setting a clean foundation for subsequent analysis.

## 2.Exploratory Data Analysis
### I. Global Correlation Mapping
We used Heatmaps to visualize linear relationships between features, identifying key factors like satisfaction and monthly income.

### II. Bivariate Discovery of the "Overwork Trap"
Through scatter plots of project counts vs. work hours, we uncovered a high-risk attrition cluster where extreme workloads lead to a "breaking point."
## 3.Feature Engineering (Core Phase)
### I. Logical Signal Transformation
We engineered the is_overworked indicator based on our EDA findings, successfully boosting the predictive correlation from 0.06 to 0.42.

### II. Optimization & Leakage Prevention
We performed target encoding and meticulously removed "Data Leakage" variables to ensure the model remains realistic and robust.
## 4.Model Building
### I. Random Forest Implementation
A Random Forest Classifier was trained to handle the complex, non-linear relationships identified during the engineering phase.

### II. Performance Metrics & Importance
The model was evaluated using confusion matrices and featur
