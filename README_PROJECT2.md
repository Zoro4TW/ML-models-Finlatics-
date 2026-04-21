# Wine Quality Prediction

**Multi-class classification model to predict wine quality ratings based on physicochemical properties.**

---

## 📋 Project Overview

This project builds a machine learning model to predict wine quality scores based on various physicochemical tests. The model helps wineries understand which chemical properties contribute most to quality ratings and can assist in quality control processes.

### Problem Statement
Predict wine quality scores (0-10 scale) using physicochemical attributes such as acidity, sugar content, pH levels, and alcohol percentage.

---

## 📊 Dataset Information

**Source:** UCI Machine Learning Repository - Wine Quality Dataset

**Dataset Variants:**
- Red Wine Dataset
- White Wine Dataset
- Combined Dataset (if applicable)

**Features (11 physicochemical properties):**
1. **Fixed Acidity** - Tartaric acid concentration (g/dm³)
2. **Volatile Acidity** - Acetic acid concentration (g/dm³)
3. **Citric Acid** - Citric acid concentration (g/dm³)
4. **Residual Sugar** - Sugar remaining after fermentation (g/dm³)
5. **Chlorides** - Salt content (g/dm³)
6. **Free Sulfur Dioxide** - SO₂ in free form (mg/dm³)
7. **Total Sulfur Dioxide** - Total SO₂ content (mg/dm³)
8. **Density** - Wine density (g/cm³)
9. **pH** - Acidity/alkalinity scale (0-14)
10. **Sulphates** - Potassium sulphate concentration (g/dm³)
11. **Alcohol** - Alcohol percentage by volume (%)

**Target Variable:** Quality score (0-10, typically 3-8 in practice)

**Dataset Size:**
- Red Wine: ~1,600 samples
- White Wine: ~4,900 samples
- Total: [Your actual dataset size]

---

## 🔬 Methodology

### 1. Data Preprocessing
- Handle missing values (if any)
- Remove duplicate entries
- Outlier detection and treatment
- Feature scaling (StandardScaler/MinMaxScaler)
- Class imbalance analysis

### 2. Exploratory Data Analysis (EDA)
- Distribution analysis of all features
- Quality score distribution (class imbalance check)
- Correlation analysis between features
- Feature relationships with target variable
- Comparison between red and white wines (if applicable)

### 3. Feature Engineering
- Created interaction features
- Polynomial features for non-linear relationships
- Binning quality scores into categories (Low/Medium/High)
- Feature selection using correlation and importance scores

### 4. Model Development

**Problem Approach:**
- Multi-class Classification (predicting exact quality scores)
- OR Binary/Ternary Classification (Low/Medium/High quality)

**Algorithms Tested:**
- Logistic Regression (baseline)
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting (XGBoost/LightGBM)
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- [Add your specific models]

**Final Model:** [Your best performing model]

**Handling Class Imbalance:**
- SMOTE (Synthetic Minority Over-sampling)
- Class weights adjustment
- Ensemble methods

### 5. Model Evaluation

**Metrics Used:**
- Accuracy
- Precision (macro/weighted average)
- Recall (macro/weighted average)
- F1-Score (macro/weighted average)
- Confusion Matrix
- Classification Report
- ROC-AUC (for binary classification variant)

---

## 📈 Results

### Model Performance

| Metric | Score |
|--------|-------|
| Accuracy | [Your score]% |
| Precision (Weighted) | [Your score]% |
| Recall (Weighted) | [Your score]% |
| F1-Score (Weighted) | [Your score]% |

### Confusion Matrix Analysis
[Add interpretation of confusion matrix - which classes are most confused]

### Key Insights

1. **Top Predictive Features:**
   - **Alcohol Content** - Strongest positive correlation with quality
   - **Volatile Acidity** - Higher values indicate lower quality
   - **Sulphates** - Important for wine preservation and quality
   - **Citric Acid** - Adds freshness to wines

2. **Quality Patterns:**
   - High-quality wines (score ≥7): Higher alcohol, lower volatile acidity
   - Low-quality wines (score ≤5): Higher volatile acidity, lower alcohol
   - Most wines fall in the 5-6 quality range (class imbalance)

3. **Red vs White Differences:** [If applicable]
   - White wines generally have higher residual sugar
   - Red wines show different acidity patterns

---

## 🛠️ Technologies Used

- **Python 3.x**
- **pandas** - Data manipulation
- **NumPy** - Numerical operations
- **scikit-learn** - Machine learning models and evaluation
- **imbalanced-learn** - SMOTE implementation (if used)
- **XGBoost/LightGBM** - Gradient boosting (if used)
- **Matplotlib/Seaborn** - Visualization
- **Jupyter Notebook** - Development environment

---

## 🚀 How to Run

### Prerequisites
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter imbalanced-learn
```

### Run the Notebook
```bash
jupyter notebook Project_2-Wine_Quality_Prediction.ipynb
```

### Dataset Setup
The Wine Quality dataset can be downloaded from:
- UCI ML Repository: https://archive.ics.uci.edu/ml/datasets/wine+quality
- Or use the dataset file included in this repository

---

## 📊 Visualizations

The notebook includes:
- Distribution plots for all physicochemical features
- Quality score distribution (bar chart)
- Correlation heatmap
- Feature importance plot
- Confusion matrix heatmap
- ROC curves (if applicable)
- Pair plots for key feature relationships

---

## 🎯 Business Applications

This model can help:
1. **Wineries** - Quality control and production optimization
2. **Sommeliers** - Understanding chemical profiles of quality wines
3. **Researchers** - Studying factors affecting wine quality
4. **Producers** - Adjusting production parameters for desired quality
5. **Quality Assurance** - Automated preliminary quality assessment

---

## 🔮 Future Improvements

- [ ] Implement deep learning models (Neural Networks)
- [ ] Add ensemble stacking techniques
- [ ] Hyperparameter optimization using GridSearchCV/Bayesian optimization
- [ ] Include additional features (grape variety, region, vintage year)
- [ ] Deploy model as web application
- [ ] Create recommendation system for wine improvement
- [ ] Cross-validation with different wine datasets
- [ ] Implement SHAP values for model interpretability

---

## 📚 Dataset Citation

```
P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis.
Modeling wine preferences by data mining from physicochemical properties.
In Decision Support Systems, Elsevier, 47(4):547-553, 2009.
```

---

## 📚 References

- UCI Machine Learning Repository - Wine Quality Dataset
- Wine quality research papers
- scikit-learn documentation
- Domain knowledge sources on wine chemistry

---

## 📝 Notes

- Quality scores are subjective and based on sensory data
- Model predictions should be used as guidance, not absolute truth
- Different wine types may require separate models
- Chemical properties alone don't capture all aspects of wine quality

---

**⭐ If you found this project insightful, please star the repository!**
