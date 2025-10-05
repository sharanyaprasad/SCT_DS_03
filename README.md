# SCT_DS_03
# 🏦 Bank Marketing Decision Tree Classifier

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0%2B-orange)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-green)](https://pandas.pydata.org/)

## 📋 Task Description

Build a **decision tree classifier** to predict whether a customer will purchase a product or service based on their demographic and behavioral data.

## 🔍 How was it done?

The **Bank Marketing dataset** from the UCI Machine Learning Repository containing 41,188 customer records was used. A decision tree classification model was built following these steps:

1. **Data Loading & Exploration** - Loaded the dataset and analyzed basic statistics
2. **Data Preprocessing** - Encoded categorical variables (job, marital status, education, etc.) using Label Encoding
3. **Train-Test Split** - Split data into 80% training and 20% testing sets
4. **Model Building** - Created a Decision Tree Classifier with max_depth=5 to prevent overfitting
5. **Evaluation** - Assessed model performance using accuracy, confusion matrix, and classification report
6. **Feature Analysis** - Identified the most important features influencing customer decisions

Python libraries including pandas, scikit-learn, matplotlib, and seaborn were used for data processing, modeling, and visualization.

## 📊 Dataset Source

**UCI Machine Learning Repository - Bank Marketing Dataset**
- **URL:** https://archive.ics.uci.edu/dataset/222/bank+marketing
- **Records:** 41,188 customers
- **Attributes:** 20 features including age, job, marital status, education, balance, contact type, and campaign details
- **Target:** Whether the client subscribed to a term deposit (yes/no)

## 💡 Key Findings

- **Test Accuracy:** ~90% - Model performs well on unseen data
- **Class Imbalance:** Only 11.3% customers subscribed to term deposits
- **Top Important Features:**
  - Duration of last contact
  - Economic indicators (euribor3m, emp.var.rate)
  - Number of previous contacts
  - Customer age
- **Decision Tree Depth:** 5 levels effectively capture patterns without overfitting
- **Model Generalization:** Similar training and testing accuracy indicates good generalization

## 🎨 Visualizations

### Confusion Matrix
Shows the model's prediction accuracy across both classes (subscribed vs not subscribed)

### Feature Importance
Identifies which customer attributes most influence subscription decisions

### Decision Tree Structure
Visual representation of the decision-making process at each node

## 🔧 Tech Stack

- **Python 3.8+**
- **Pandas** - Data manipulation
- **Scikit-learn** - Machine learning model
- **Matplotlib** - Data visualization
- **Seaborn** - Enhanced visualizations
- **NumPy** - Numerical operations
- **Jupyter Notebook** - Interactive analysis

## 📈 Results Summary

| Metric | Value | Description |
|--------|-------|-------------|
| **Total Records** | 41,188 | Complete dataset size |
| **Training Set** | 32,950 (80%) | Data used for training |
| **Testing Set** | 8,238 (20%) | Data used for evaluation |
| **Test Accuracy** | ~90% | Model performance |
| **Subscribed (Yes)** | 4,640 (11.3%) | Positive class |
| **Not Subscribed (No)** | 36,548 (88.7%) | Negative class |
| **Tree Depth** | 5 levels | Complexity control |
| **Important Features** | Duration, Economic indicators | Top predictors |
