Stack Overflow Developer Survey Analysis
Udacity Data Science Nanodegree — Write a Data Science Blog Post
![Developer Survey Banner](https://img.shields.io/badge/Python-3.11-blue) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange) ![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-green) ![CRISP--DM](https://img.shields.io/badge/Process-CRISP--DM-purple)
---
Motivation
Every year Stack Overflow surveys hundreds of thousands of developers worldwide. This project digs into that data to answer three practical questions that matter to developers and employers alike:
What factors most influence a developer's annual salary?
How does education level relate to job satisfaction?
Can we predict whether a developer earns above the median salary?
---
Libraries Used
Library	Purpose
`pandas`	Data loading, manipulation, and analysis
`numpy`	Numerical operations and array handling
`matplotlib`	Base plotting framework
`seaborn`	Statistical data visualization
`scikit-learn`	Machine learning — preprocessing, modeling, evaluation
`nbformat`	Jupyter notebook creation utilities
---
Repository Files
File	Description
`StackOverflow_Developer_Survey_Analysis.ipynb`	Main Jupyter notebook — full CRISP-DM analysis with EDA, modeling, and prediction
`survey_results_public.csv`	Dataset used in the analysis (representative Stack Overflow survey sample)
`README.md`	This file — project overview and instructions
`plot_salary_distribution.png`	Histogram of annual salary (raw and log-transformed)
`plot_salary_by_country.png`	Median salary by country bar chart
`plot_education_satisfaction.png`	Education level vs. job satisfaction
`plot_remote_work.png`	Remote work distribution and salary impact
`plot_languages.png`	Most used programming languages
`plot_correlation.png`	Correlation heatmap of numerical features
`plot_pca.png`	PCA scree plot and cumulative variance
`plot_evaluation.png`	Confusion matrices and ROC curve comparison
`plot_feature_importance.png`	Random Forest feature importance
`plot_sarah_prediction.png`	Scenario prediction visualization
---
Summary of Results
Country is the dominant predictor of salary — accounting for the largest share of the Random Forest model's decisions. A developer in the US earns a median salary roughly 5× that of a developer in India.
Experience matters significantly — years of professional coding is the second most important feature.
Education and job satisfaction have a modest but non-linear relationship. Doctoral degree holders report slightly higher satisfaction, but the difference between education groups is small.
The Random Forest model achieved strong accuracy and AUC scores, substantially outperforming the logistic regression baseline.
Remote work correlates with slightly higher median salaries, likely because remote-friendly roles skew toward higher-paying companies.
---
How to Run
```bash
# 1. Clone the repository
git clone https://github.com/your-username/stackoverflow-survey-analysis.git
cd stackoverflow-survey-analysis

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn nbformat jupyter

# 3. Launch Jupyter
jupyter notebook StackOverflow_Developer_Survey_Analysis.ipynb
```
---
Acknowledgments
Stack Overflow Annual Developer Survey — the inspiration and structure for this dataset
Udacity Data Science Nanodegree — project framework and CRISP-DM guidance
scikit-learn — machine learning library documentation
