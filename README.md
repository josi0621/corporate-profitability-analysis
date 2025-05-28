# 📊 What Drives Corporate Profitability?

## 🧠 Introduction
This project explores the financial factors that influence company profitability using data from the *Corporate Credit Rating with Financial Ratios* dataset on Kaggle. We focus on predicting two key financial performance metrics:

- **Return on Assets (ROA)**
- **Net Profit Margin**

Our goal is to understand which financial ratios most strongly predict profitability.

---

## 📁 Data Overview

- **Dataset**: Corporate Credit Rating with Financial Ratios (Kaggle)
- **Rows**: ~7800
- **Columns**: Financial ratios such as ROA, ROE, Net Profit Margin, Debt/Equity, Operating Margin, etc.
- **No missing values** in selected columns for analysis.

---

## 🧹 Data Cleaning & Selection

We selected the following columns for this analysis:

- ROA – Return On Assets
- Net Profit Margin
- Operating Margin
- Gross Margin
- Debt/Equity Ratio
- Current Ratio

We confirmed there were no missing values and created a clean subset for modeling.

---

## 📊 Exploratory Data Analysis

We used correlation analysis and scatter plots to explore relationships between variables.

### 🔥 Key Findings:
- **ROA** is highly correlated with Net Profit Margin and Operating Margin.
- **Net Profit Margin** is strongly predicted by ROA and Operating Margin.

---

## 🤖 Modeling Profitability Metrics

We used linear regression models to predict both ROA and Net Profit Margin.

### 📈 Model 1: Predicting ROA
- **Features**: Net Profit Margin, Operating Margin, Debt/Equity Ratio, Gross Margin, Current Ratio
- **R² Score**: ~0.627
- **Top Predictors**: Net Profit Margin, Operating Margin

### 📈 Model 2: Predicting Net Profit Margin
- **Features**: ROA, Operating Margin, Debt/Equity Ratio, Gross Margin, Current Ratio
- **R² Score**: ~0.855
- **Top Predictors**: ROA, Operating Margin

---

## ✅ Conclusion

- Profitability is most closely linked to operational and asset efficiency.
- ROA and Operating Margin are consistently strong predictors.
- Linear models are effective for explaining a large portion of profitability variance.

---

## 🚀 Next Steps

- Explore industry-specific patterns
- Use regularization or tree-based models
- Expand to include time-series trends or macroeconomic indicators

---

## 📎 References

- Kaggle Dataset: [Corporate Credit Rating with Financial Ratios](https://www.kaggle.com/datasets/kirtandelwadia/corporate-credit-rating-with-financial-ratios)
- Scikit-learn, pandas, seaborn
