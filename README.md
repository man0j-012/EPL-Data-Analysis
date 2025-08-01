Comprehensive Analysis of EPL Match Data Using Machine Learning

# ⚽ English Premier League (EPL) Match Data Analytics

## 📌 Overview

This project explores English Premier League (EPL) match data through deep statistical analysis and machine learning modeling. By examining trends across match formations, home-field advantage, shooting efficiency, and expected goals (xG), we aim to uncover actionable insights and predict match outcomes with meaningful accuracy.

Designed for sports analysts, data scientists, and machine learning enthusiasts, this project demonstrates the full data science lifecycle — from web scraping and EDA to hypothesis testing and predictive modeling.

---

## 🗂 Repository Structure

epl-match-analytics/
│
├── data/ # Raw and processed match data
│ └── matches.csv
│
├── scripts/ # Web scraping, EDA, hypothesis testing
│ ├── data_collection.ipynb
│ ├── data_analysis.ipynb
│ └── hypothesis_testing.ipynb
│
├── models/ # Machine learning models and evaluations
│ └── ml_models.ipynb
│
├── reports/ # Final report and progress updates
│ ├── cs_418_final_report.pdf
│ └── progress_report_3.ipynb
│
├── docs/ # Optional notes, visuals, and charts
│
├── README.md # You're here!
├── requirements.txt # All project dependencies
└── .gitignore # Git exclusions

---

## 🧠 Key Objectives

- Collect and preprocess EPL match data from trusted public sources
- Explore player and team statistics through rich visualizations
- Validate key questions using statistical hypothesis testing
- Predict match outcomes using multiple machine learning models
- Rank features by importance and model performance
- Present findings through reports and performance metrics

---

## 🛠 Tools & Technologies

| Category        | Stack                              |
| --------------- | ---------------------------------- |
| **Scraping**    | BeautifulSoup, Requests            |
| **EDA**         | Pandas, NumPy, Matplotlib, Seaborn |
| **Modeling**    | Scikit-learn, TensorFlow           |
| **Environment** | Jupyter Notebooks, Markdown        |

---

## 📥 Data Pipeline

1. **Source**: Match data scraped from [fbref.com](https://fbref.com/) and Stathead (requires subscription).
2. **Processing**: CSV parsing, null handling, feature engineering.
3. **Feature Engineering**:
   - `Avg_Goals_Scored_3`: Goals average in last 3 matches
   - `Goal_Efficiency`: Goals scored per shot
   - `Shooting_Accuracy`: Shots on target percentage

---

## 📊 Exploratory Analysis

- 5,000+ EPL matches across 7 seasons analyzed
- Visuals:
  - 🔥 Heatmaps (correlations)
  - 📊 Radar Charts (team profiles)
  - ⚽ Scatter plots (xG vs GF)
  - 🏟️ Bar plots (formation, home vs away)

---

## 🔬 Hypothesis Testing

| Hypothesis                                    | Test Used         |
| --------------------------------------------- | ----------------- |
| Home advantage influences win rate            | One-sample t-test |
| Higher shooting accuracy correlates with wins | Binomial test     |
| Formations influence match outcomes           | Chi-square test   |

All results include p-values, confidence intervals, and effect size discussions.

---

## 🤖 Machine Learning Models

| Model             | Accuracy   | Notes                                        |
| ----------------- | ---------- | -------------------------------------------- |
| Gradient Boosting | **61.46%** | Captured nonlinear patterns best             |
| Random Forest     | ~60%       | Robust and interpretable feature importances |
| Neural Networks   | ~58%       | High variance, requires tuning               |
| Others            | Varying    | Logistic Regression, SVM, Decision Trees     |

> Evaluated using confusion matrices, ROC curves, precision, recall, and F1-score.

---

## ✅ Key Findings

- **Gradient Boosting** provided the most consistent performance.
- **Shooting efficiency** and **formations** were statistically significant predictors.
- **Home teams** consistently showed a performance edge.

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/epl-match-analytics.git
cd epl-match-analytics
```

2. Install dependencies
   pip install -r requirements.txt

3. Run notebooks
   Start with: scripts/data_analysis.ipynb

Test insights: scripts/hypothesis_testing.ipynb

Build models: models/ml_models.ipynb

Optional: To regenerate data, run scripts/data_collection.ipynb (Stathead access required).

📑 Documentation
📄 Final Report: cs_418_final_report.pdf

🧾 Progress Report: progress_report_3.ipynb

📘 Summary: See README.md

🧠 Learning Outcomes
Built a full-stack analytics pipeline from data scraping to model evaluation

Applied real-world machine learning to sports data

Practiced statistical validation of hypotheses

Learned the importance of explainability, visualization, and model comparison

🙏 Acknowledgments
Thanks to fbref and Stathead for the data.

Special appreciation to the University of Illinois at Chicago CS418 Faculty for their mentorship and project support.

🔖 Tags
epl · football-analytics · machine-learning · sports-data · hypothesis-testing · gradient-boosting · python · scikit-learn · data-science
Project Overview
This repository contains the work of our project on analyzing English Premier League (EPL) football matches using machine learning techniques. Our goal is to enhance strategic decision-making and improve game outcomes by exploring the predictive power of machine learning in sports analytics.

Purpose
The project aims to:

Analyze various match-related statistics to determine influential factors on match results, such as team formations, home advantage, and shot efficiency.
Develop predictive models using machine learning techniques like Logistic Regression, Random Forest, and Gradient Boosting to forecast match outcomes.
Repository Structure
data/: Contains the raw and processed datasets used in our analyses.
docs/: Documentation related to the project and findings.
src/: Source code for the data preprocessing, exploratory data analysis, hypothesis testing, and machine learning models.
notebooks/: Jupyter notebooks detailing the exploratory data analysis and model development processes.
results/: Visualizations and output files from our analyses.
Methodology
Data Collection and Preprocessing: Using Beautiful Soup for web scraping data from the ‘fbref’ website, followed by data cleaning and preprocessing.
Exploratory Data Analysis (EDA): Initial patterns, trends, and anomalies within the data were explored to understand the impact of football formations, goal differentials, and more.
Hypothesis Testing: Evaluating theories like the influence of higher shot counts on winning games and the statistical significance of 'home advantage'.
Model Development and Validation: Machine learning models were developed and validated using performance metrics like accuracy, precision, recall, and F1 score.
Tools and Technologies
Python: For data scraping, preprocessing, and machine learning.
Beautiful Soup: Used for web scraping.
Pandas, NumPy: Data manipulation and analysis.
Matplotlib, Seaborn: For data visualization.
Scikit-learn: For implementing machine learning models.
