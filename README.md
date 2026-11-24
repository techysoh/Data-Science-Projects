# Data Science & Machine Learning Projects

This repository contains two Python projects focused on **employee
attrition prediction** and **apparel sales analysis**. Both projects use
Jupyter Notebook and common Python data-analysis libraries.

------------------------------------------------------------------------

## Repository Contents

``` text
Data-Science-Projects/
├── Employee-Turnover/
│   ├── Employee_Turnover.ipynb
│   └── HR_comma_sep.csv
├── Apparel-Sales-Analysis/
│   ├── aimlihfc_project2.ipynb
│   └── AusApparalSales4thQrt2020.csv
└── README.md
```


------------------------------------------------------------------------

# Project 1: Employee Turnover Prediction

## Overview

This project explores employee turnover using HR data and builds
machine-learning classification models to estimate whether an employee
is likely to leave the organization. It also groups employees who left
into clusters based on satisfaction and evaluation scores and assigns
turnover-risk categories to test records.

## Objectives

-   Explore and understand the HR dataset.
-   Examine employee turnover patterns and relationships among
    variables.
-   Segment employees who left using K-Means clustering.
-   Train and compare classification models.
-   Estimate employee turnover probabilities and assign risk zones.
-   Present possible HR retention actions for each risk zone.

## Workflow

1.  **Data loading and inspection:** Load the CSV file and inspect its
    structure, missing values, duplicates, descriptive statistics and
    unique values.
2.  **Data cleaning:** Remove duplicate records.
3.  **Exploratory data analysis:** Visualize turnover distribution,
    correlations, satisfaction, evaluation scores, monthly working hours
    and project counts.
4.  **Clustering:** Standardize satisfaction and last-evaluation values
    for employees who left, then apply K-Means with three clusters.
5.  **Preprocessing:** Separate the target column (`left`) from the
    features and one-hot encode categorical variables.
6.  **Train/test split:** Split the data into training and test sets
    using stratification.
7.  **Class balancing:** Apply SMOTE to address class imbalance in the
    training process.
8.  **Model development:** Compare Logistic Regression, Random Forest
    and Gradient Boosting using stratified 5-fold cross-validation with
    F1 score.
9.  **Evaluation:** Evaluate models using accuracy, precision, recall,
    F1 score, ROC-AUC, confusion matrices and ROC curves.
10. **Risk analysis:** Select the model with the highest test F1 score,
    calculate turnover probabilities and classify predictions into Safe,
    Low, Medium and High risk zones.

## Technologies and Libraries

-   Python
-   Jupyter Notebook
-   Pandas and NumPy
-   Matplotlib and Seaborn
-   Scikit-learn
-   imbalanced-learn (SMOTE)

## Dataset

The notebook expects a file named `HR_comma_sep.csv`. Ensure that you
have permission to share the dataset before committing it to a public
repository.

## How to Run

1.  Install Python and Jupyter Notebook, or use Google Colab.

2.  Install the required libraries:

    ``` bash
    pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn jupyter
    ```

3.  Place `HR_comma_sep.csv` in the notebook's working directory.

4.  Open `Employee_Turnover.ipynb`.

5.  Run the notebook cells from top to bottom.

## Output

The notebook produces exploratory charts, K-Means cluster summaries,
cross-validation comparisons, model evaluation reports, confusion
matrices, ROC curves, turnover probabilities and risk-zone summaries.
Actual performance values depend on the dataset and execution
environment; see the notebook outputs for the measured results.

------------------------------------------------------------------------

# Project 2: Apparel Sales Analysis --- Fourth Quarter 2020

## Overview

This project analyses apparel sales data for the fourth quarter of 2020
(October, November and December). It uses data cleaning, date-based
grouping, summary tables and visualizations to explore sales and unit
trends across months, states, customer groups and time categories.

## Objectives

-   Inspect and prepare the apparel sales dataset.
-   Summarize sales and units sold over time.
-   Compare October, November and December 2020.
-   Explore sales by state and customer group.
-   Examine sales patterns across the available time categories.
-   Use visualizations and pivot tables to summarize the data.

## Workflow

1.  **Data loading:** Load the CSV file and parse the `Date` column as
    dates.
2.  **Data inspection and cleaning:** Review data types and missing
    values, fill missing numeric values with column means, and remove
    remaining rows with missing values.
3.  **Numerical preprocessing:** Select numerical columns and apply
    Min-Max normalization.
4.  **Date-based analysis:** Aggregate sales and units by date and
    separate the data into October, November and December.
5.  **Trend visualization:** Plot daily sales and unit trends, and use
    boxplots to inspect monthly distributions.
6.  **Monthly comparison:** Compare total sales and daily units across
    the three months.
7.  **Category analysis:** Aggregate sales by state and group, and
    create pivot tables for comparisons.
8.  **Time analysis:** Summarize sales and units by the dataset's `Time`
    category and visualize the mean sales distribution.

## Technologies and Libraries

-   Python
-   Jupyter Notebook
-   Pandas and NumPy
-   Matplotlib and Seaborn
-   Scikit-learn (`MinMaxScaler`)

## Dataset

The notebook expects `AusApparalSales4thQrt2020.csv`, containing the
fourth-quarter 2020 apparel sales data. The original notebook uses the
path `/content/AusApparalSales4thQrt2020.csv`, which is suitable for
Google Colab. Update the path if running locally. Confirm that the
dataset may be redistributed before uploading it to a public repository.

## How to Run

1.  Install Python and Jupyter Notebook, or use Google Colab.

2.  Install the required libraries:

    ``` bash
    pip install pandas numpy matplotlib seaborn scikit-learn jupyter
    ```

3.  Place `AusApparalSales4thQrt2020.csv` in the location used by the
    notebook, or update the CSV path.

4.  Open `aimlihfc_project2.ipynb`.

5.  Run the notebook cells from top to bottom.

## Output

The notebook produces monthly sales and unit summaries, daily trend
charts, boxplots, state/group pivot tables and visualizations of sales
by group and time category. Refer to the notebook outputs for the actual
values and findings.

------------------------------------------------------------------------

## Skills Demonstrated

-   Data cleaning and preprocessing
-   Exploratory data analysis (EDA)
-   Data visualization
-   Feature encoding and scaling
-   Classification and model evaluation
-   Imbalanced-class handling with SMOTE
-   K-Means clustering
-   Time-based aggregation
-   Pivot tables and business-oriented analysis

## Author

**Soham Mondal**

These projects are presented for learning and portfolio purposes. Please
review the notebooks and dataset licensing/redistribution terms before
using or sharing the contents.
