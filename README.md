# Student Engagement Analysis and Retention Prediction Portfolio

**Author:** Ihor Melashchenko  
**Student ID:** C00290950  
**Module:** Data Science and Machine Learning 1  
**Institution:** South East Technological University  
**Date:** November 2025

## 📋 Overview

This portfolio demonstrates data science and machine learning techniques applied to student engagement analysis within the context of the **University App** (my final-year project). The work combines unsupervised and supervised learning approaches to extract actionable insights from student interaction data.

### Project Components

1. **Clustering App Usage Patterns** - Unsupervised learning to identify natural groupings of students based on their app interaction behaviors
2. **Predicting Student Retention Risk** - Supervised learning models to forecast dropout risk using behavioral and academic metrics

## 🎯 Objectives

- Simulate realistic datasets representing University App usage and academic engagement
- Perform exploratory data analysis (EDA) and clustering to segment students
- Develop and evaluate classification models for dropout risk prediction
- Interpret key features influencing student engagement
- Present results through clear visualizations and structured documentation
- Demonstrate professional data science workflow and reproducible research practices

## 📊 Datasets

### Primary Data
- **Synthetic dataset** representing 400 anonymized student records
- Features include app usage metrics (logins, digital ID scans, timetable views, notifications, session duration)
- Academic metrics (attendance rate, assignment submission rate, GPA)

### Generated Files
- `data/university_app_usage_clusters.csv` - Clustered app usage patterns
- `data/student_retention_dataset.csv` - Labeled retention risk data

## 🛠️ Technologies & Tools

### Programming Language
- Python 3.x

### Development Environment
- Jupyter Notebook / JupyterLab

### Core Libraries
- **Data Processing**: NumPy, Pandas
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn, XGBoost
- **Statistical Analysis**: SciPy

### Version Control
- Git & GitHub

## 📁 Project Structure

```
DS-and-ML-1-CA/
│
├── README.md                          # Project documentation
├── data/                              # Data files
│   ├── student_retention_dataset.csv
│   └── university_app_usage_clusters.csv
│
└── notebooks/                         # Jupyter notebooks
    ├── clustering_app_usage_patterns.ipynb
    └── predicting_retention_risk.ipynb
```

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.x installed.

### Running the Notebooks

1. Clone the repository:
```bash
git clone https://github.com/baldeagle0125/DS-and-ML-1-CA.git
cd DS-and-ML-1-CA
```

2. Create and activate a virtual environment (recommended):
```bash
python3 -m venv venv
source venv/bin/activate  # macOS/Linux
# OR
venv\Scripts\activate     # Windows
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

4. Launch Jupyter Notebook:
```bash
jupyter notebook
```

5. Navigate to the `notebooks/` directory and open:
   - `clustering_app_usage_patterns.ipynb` - Start here for unsupervised learning analysis
   - `predicting_retention_risk.ipynb` - Continue with supervised learning predictions

### Execution Order

**Recommended sequence:**
1. Run `clustering_app_usage_patterns.ipynb` first to understand student segments
2. Then run `predicting_retention_risk.ipynb` to build predictive models

Both notebooks are self-contained and can be executed cell-by-cell.

## 📈 Methodology

### Part 1: Clustering App Usage Patterns

**Approach:** Unsupervised Learning (K-Means Clustering)

1. **Data Generation** - Simulate 400 student records with 6 app usage features
2. **Exploratory Analysis** - Statistical summaries and correlation analysis
3. **Feature Scaling** - StandardScaler normalization
4. **Optimal k Selection** - Elbow Method analysis
5. **Clustering** - K-Means with k=3 clusters
6. **Evaluation** - Silhouette Score validation
7. **Visualization** - PCA dimensionality reduction for 2D visualization
8. **Interpretation** - Identify behavioral patterns (High/Moderate/Low engagement)

**Key Insights:**
- Three distinct engagement clusters identified
- Clear separation between highly engaged and at-risk students
- Session duration and login frequency are key differentiators

### Part 2: Predicting Student Retention Risk

**Approach:** Supervised Learning (Classification)

1. **Data Preparation** - 9 features (app usage + academic metrics)
2. **Target Creation** - Binary dropout risk label based on combined thresholds
3. **Train-Test Split** - 80/20 split with stratification
4. **Model Training** - Three algorithms:
   - Logistic Regression (baseline)
   - Random Forest (ensemble)
   - XGBoost (gradient boosting)
5. **Evaluation** - Accuracy, Precision, Recall, F1-Score, ROC-AUC
6. **Feature Importance** - Identify critical predictors
7. **Validation** - Confusion matrix analysis

**Key Results:**
- High prediction accuracy across all models (typically >85%)
- Academic metrics (GPA, attendance) are strongest predictors
- App engagement patterns provide additional predictive value
- Random Forest and XGBoost outperform baseline Logistic Regression

## 🔍 Key Findings

### Student Engagement Clusters

| Cluster | Behavior Pattern | Characteristics |
|---------|------------------|-----------------|
| 0 | High Engagement | Frequent logins, event participation, long sessions |
| 1 | Moderate Engagement | Regular users, balanced activity levels |
| 2 | Low Engagement | Minimal app usage, potential at-risk indicators |

### Predictive Insights

- **Top Risk Factors:**
  1. Low GPA (< 2.2)
  2. Poor attendance rate (< 75%)
  3. Low assignment submission (< 60%)
  4. Infrequent app logins (< 6/week)

- **Model Performance:** All models achieved strong metrics, validating the predictive value of combined behavioral and academic data

## 💡 Practical Applications

1. **Early Warning System** - Identify at-risk students proactively
2. **Targeted Interventions** - Design support programs based on cluster characteristics
3. **App Feature Optimization** - Improve engagement features that correlate with retention
4. **Resource Allocation** - Prioritize support for high-risk student segments
5. **Data-Driven Policy** - Evidence-based student success strategies

## 📝 Documentation

Each Jupyter notebook includes:
- Comprehensive markdown explanations
- Code comments and documentation
- Visualizations with interpretations
- Section summaries and conclusions

## 🔗 Related Work

This portfolio connects to my final-year project, the **University App**, which provides students with:
- Digital student ID
- Timetable management
- Event notifications
- Campus services integration

The analytics insights developed here could inform future app development and student support initiatives.

## 🎓 Academic Context

**Assessment Details:**
- Module: Data Science and Machine Learning 1
- Value: 60% of module grade
- Components:
  - Portfolio Specification (5%)
  - Single Portfolio Item (10%)
  - Final Portfolio Submission (35%)
  - In-Class Presentation (10%)

**Note:** This portfolio uses synthetic data for demonstration purposes. Future work could incorporate real anonymized student data (with appropriate ethical approval) to validate findings.

**Last Updated:** November 28, 2025
