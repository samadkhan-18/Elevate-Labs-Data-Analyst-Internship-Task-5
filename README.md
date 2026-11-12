# Elevate-Labs-Data-Analyst-Internship-Task-5
## Task 5: Exploratory Data Analysis (EDA) on the Titanic Dataset

**Data Analyst Internship - Elevate Labs**
**Author:** Ahemad Maheed Khan ([@samadkhan-18](https://github.com/samadkhan-18))

## Objective
Extract insights from the Titanic dataset using visual and statistical exploration, and identify patterns, trends and anomalies related to passenger survival.

## Tools Used
- Python
- Pandas and NumPy (data handling)
- Matplotlib and Seaborn (visualization)
- Jupyter Notebook in VS Code

## Dataset
Titanic passenger dataset (`titanic.csv`), with columns such as Survived, Pclass, Sex, Age, SibSp, Parch, Fare, Cabin and Embarked.

## Steps Performed
1. **Data inspection:** used `head()`, `shape`, `info()`, `describe()` and `value_counts()` to understand structure, data types and distributions.
2. **Data cleaning:**
   - Filled missing `Age` values with the median (robust to outliers and skew).
   - Filled missing `Embarked` values with the mode.
   - Filled missing `Cabin` values with "Unknown" instead of dropping the column, because about 77% of values were missing and the missingness itself is informative.
   - Checked for duplicate rows.
3. **Univariate analysis:** histograms for Age and Fare; count plots for Survived, Pclass and Sex.
4. **Bivariate analysis:** survival rate by Sex, Pclass, Embarked and cabin availability; boxplots of Fare by Pclass and Age by Survived; scatterplot of Age vs Fare colored by Survived.
5. **Multivariate analysis:** correlation heatmap, pairplot, and survival by Pclass and Sex together.
6. **Observations:** a written observation was added under every visual, followed by a summary of findings.

## Key Findings
- **Sex:** women survived at a far higher rate than men.
- **Passenger class:** first-class passengers had a higher survival rate than third-class passengers.
- **Fare:** the distribution is heavily right-skewed with high-fare outliers, mostly in first class.
- **Age:** most passengers were young adults; children showed a somewhat higher survival rate.
- **Cabin:** passengers with a recorded cabin were mostly first class and survived more often.
- **Correlation:** Pclass is negatively correlated with Fare and with Survived.

## Repository Structure
```
Eda-Titanic-Task5/
├── notebook.ipynb            # Full EDA notebook with code and observations
├── titanic.csv               # Dataset
├── EDA_Titanic_Report.pdf    # PDF report of findings
├── images/                   # Saved plots
└── README.md
```

## How to Run
1. Clone the repository.
2. Install the requirements: `pip install pandas numpy matplotlib seaborn jupyter`
3. Open `notebook.ipynb` and run all cells.
