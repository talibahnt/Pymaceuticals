# Pymaceuticals
Background
You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.
Prepare the data.

Generate summary statistics.

Create bar charts and pie charts.

Calculate quartiles, find outliers, and create a box plot.

Create a line plot and a scatter plot.

Calculate correlation and regression.

Submit your final analysis.

 ## Pymaceuticals: Anti-Cancer Drug Clinical Study Analysis
📌 Executive Summary
Pymaceuticals, Inc. recently completed a 45-day animal study evaluating potential treatments for Squamous Cell Carcinoma (SCC), a common form of skin cancer. In this trial, 249 mice diagnosed with SCC tumors received treatment across various drug regimens. Tumor progression was monitored and recorded over time.

This project delivers a comprehensive technical analysis evaluating the performance of Pymaceuticals’ flagship drug candidate, Capomulin, relative to rival treatment regimens (including Ramicane, Infubinol, and Ceftamin).

## 🛠️ Key Analytical TasksData Preparation & Cleaning:
Combined mouse metadata and study results into a unified dataset.
Identified and removed duplicate records (e.g., duplicate timepoints for mouse ID g989).
Cleaned the dataset down to 248 unique, valid subject mice.

# Summary Statistics:
Calculated mean, median, variance, standard deviation, and SEM (Standard Error of the Mean) for tumor volume across all drug regimens.

# Visualizations & Demographics:
Bar Charts: Displayed the total number of observed mouse timepoints for each drug regimen using both Pandas and Matplotlib.Pie Charts: Evaluated the distribution of female vs. male mice across the study population.

# Quartiles, Outliers, & Box Plots:
Isolated final tumor volumes for the top four treatment regimens (Capomulin, Ramicane, Infubinol, and Ceftamin).Computed Interquartile Range (IQR) and established potential statistical outliers across regimens.Generated a comparative Box Plot highlighting distribution and potential outliers.

# Advanced Statistical Modeling:
Line Plot: Tracked tumor volume over time for a single mouse treated with Capomulin (e.g., Mouse ID l509).
Scatter Plot: Compared average mouse weight against average tumor volume for the Capomulin group.
Correlation & Linear Regression: Calculated Pearson’s correlation coefficient ($r$) and fit a linear regression model to quantify the relationship between mouse weight and tumor responsiveness.

# 📈 Key Findings & Study Insights
Top Performers: Capomulin and Ramicane demonstrated significant effectiveness in reducing SCC tumor volume over the 45-day trial period compared to placebo and other regimens.
Outlier Analysis: Across the top four regimens, only Infubinol contained a single statistically significant outlier (Mouse ID c451), while Capomulin and Ramicane exhibited highly consistent, reproducible outcomes.
Weight vs. Tumor Volume Correlation: A strong positive correlation ($r \approx 0.84$) exists between mouse weight and average tumor volume within the Capomulin regimen. Higher body mass directly corresponds to larger average tumor volumes, suggesting dosage adjustments by weight may be worth investigating in future trials.

## 📂 Repository Structure
Plaintext
Pymaceuticals/
│
├── Pymaceuticals/
│   ├── data/
│   │   ├── Mouse_metadata.csv      # Subject demographical & baseline data
│   │   └── Study_results.csv       # Timepoint measurements and tumor metrics
│   └── pymaceuticals_starter.ipynb # Main Jupyter Notebook containing analysis & charts
│
├── README.md                       # Technical documentation & project summary
└── .gitignore                      # Standard python/Jupyter gitignore rules
## 🚀 Getting Started
# Prerequisites
Make sure you have Python installed along with the necessary data science tools:

# Bash
pip install pandas matplotlib scipy notebook
Running the Analysis
Clone the repository:

# Bash
git clone https://github.com/talibahnt/Pymaceuticals.git
cd Pymaceuticals
Launch Jupyter Notebook:

# Bash
jupyter notebook Pymaceuticals/pymaceuticals_starter.ipynb
Run all cells sequentially to reproduce tables, statistical models, and visualizations.
