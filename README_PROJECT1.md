# Facebook Live Sellers - Sales Prediction

**Regression model to predict sales performance for Facebook Live sellers based on engagement metrics and video characteristics.**

---

## 📋 Project Overview

This project analyzes Facebook Live selling sessions to predict total sales amounts. The model helps sellers understand which factors drive sales performance and optimize their live streaming strategies.

### Problem Statement
Predict the total sales generated from a Facebook Live selling session based on:
- Viewer engagement metrics (likes, comments, shares)
- Video characteristics (duration, time of day)
- Seller performance indicators
- Audience reach statistics

---

## 📊 Dataset Information

**Source:** [Specify dataset source - e.g., UCI ML Repository, Kaggle, etc.]

**Features:**
- **Engagement Metrics:** Number of reactions, comments, shares
- **Reach Metrics:** Total reach, page followers
- **Video Attributes:** Duration, post type, published time
- **Performance Metrics:** Previous sales history, seller rating

**Target Variable:** Total sales amount (continuous variable)

**Dataset Size:** [Number of records] × [Number of features]

---

## 🔬 Methodology

### 1. Data Preprocessing
- Handle missing values using appropriate imputation strategies
- Remove duplicate entries
- Detect and handle outliers
- Feature scaling and normalization

### 2. Exploratory Data Analysis (EDA)
- Distribution analysis of sales and engagement metrics
- Correlation analysis between features and target variable
- Time-based patterns (day of week, time of day effects)
- Visualization of key relationships

### 3. Feature Engineering
- Created interaction features (e.g., engagement rate = reactions/reach)
- Temporal features (hour of day, day of week)
- Aggregated historical performance metrics
- Log transformations for skewed features

### 4. Model Development
**Algorithms Tested:**
- Linear Regression (baseline)
- Ridge/Lasso Regression (regularized models)
- Random Forest Regressor
- Gradient Boosting (XGBoost/LightGBM)
- [Add your specific models]

**Final Model:** [Your best performing model]

### 5. Model Evaluation
**Metrics Used:**
- R² Score (Coefficient of Determination)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)

---

## 📈 Results

### Model Performance

| Metric | Score |
|--------|-------|
| R² Score | [Your score] |
| RMSE | [Your score] |
| MAE | [Your score] |
| MAPE | [Your score]% |

### Key Insights

1. **Top Predictive Features:**
   - [Feature 1 - e.g., Number of comments]
   - [Feature 2 - e.g., Video duration]
   - [Feature 3 - e.g., Time of broadcast]

2. **Engagement Impact:**
   - Higher comment-to-view ratio strongly correlates with increased sales
   - Peak sales occur during [specific time periods]

3. **Seller Strategies:**
   - Videos longer than [X] minutes show diminishing returns
   - Optimal posting time: [Your findings]

---

## 🛠️ Technologies Used

- **Python 3.x**
- **pandas** - Data manipulation
- **NumPy** - Numerical operations
- **scikit-learn** - Model training and evaluation
- **XGBoost/LightGBM** - Gradient boosting (if used)
- **Matplotlib/Seaborn** - Visualization
- **Jupyter Notebook** - Development environment

---

## 🚀 How to Run

### Prerequisites
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

### Run the Notebook
```bash
jupyter notebook Project_1-Facebook_Live_Sellers_Sales_Prediction.ipynb
```

### Dataset Setup
Place the dataset file in the same directory or update the file path in the notebook.

---

## 📊 Visualizations

The notebook includes:
- Distribution plots for sales and engagement metrics
- Correlation heatmap
- Feature importance plot
- Actual vs. Predicted sales scatter plot
- Residual analysis plots

---

## 🎯 Business Applications

This model can help:
1. **Sellers** optimize their live streaming strategy
2. **Platform owners** understand engagement drivers
3. **Marketing teams** identify high-potential time slots
4. **Content creators** plan content based on sales predictions

---

## 🔮 Future Improvements

- [ ] Incorporate sentiment analysis from comments
- [ ] Add seasonal and holiday effects
- [ ] Implement ensemble methods for better predictions
- [ ] Deploy as a real-time prediction API
- [ ] Create a Streamlit dashboard for interactive predictions
- [ ] A/B testing framework for strategy optimization

---

## 📚 References

- [Link to dataset source]
- [Relevant research papers]
- [Documentation references]

---

## 📝 Notes

- This project was developed as part of the Finlatics program
- Model performance may vary with different datasets
- Always validate predictions with domain experts

---

**⭐ If you found this project helpful, please star the repository!**
