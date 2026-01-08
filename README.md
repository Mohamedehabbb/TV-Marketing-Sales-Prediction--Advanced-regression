# 📺 TV Marketing Sales Prediction — Data Science Project

## 👋 Project Introduction

This project focuses on analyzing **TV Marketing (Advertising) data** to understand how advertising budgets across different channels affect **product sales**.

The project is treated as a **real-world business problem**, following a structured **Data Science workflow** from problem definition to model evaluation and visualization.

---

## ❓ Problem Statement

Companies spend large budgets on advertising, but not all channels contribute equally to sales.

The key business question is:

> **How do TV, Radio, and Newspaper advertising budgets influence sales, and how accurately can we predict sales using regression models?**

This is formulated as a **supervised regression problem**, where the goal is to predict a continuous target variable (Sales).

---

## 🎯 Project Objectives

* Understand the relationship between advertising channels and sales
* Build reliable regression models
* Compare different modeling techniques
* Control overfitting and improve generalization
* Communicate results through clear visualizations

---

## 🧠 Dataset Description

**Dataset:** Advertising / TV Marketing Dataset

| Feature   | Description                  |
| --------- | ---------------------------- |
| TV        | TV advertising budget        |
| Radio     | Radio advertising budget     |
| Newspaper | Newspaper advertising budget |
| Sales     | Product sales                |

**Dataset Characteristics:**

* Numerical features only
* No missing values
* Small but highly interpretable dataset
* Business-oriented

---

## 🔄 Methodology & Step-by-Step Workflow

The project follows a **structured Data Science lifecycle**, where each step builds upon the previous one.

---

### 1️⃣ Data Understanding & Exploratory Data Analysis (EDA)

**What we did:**

* Loaded the dataset and inspected its structure
* Checked for missing values and data types
* Analyzed summary statistics
* Visualized relationships between advertising channels and sales

**Key Findings:**

* TV advertising has the strongest positive relationship with sales
* Radio advertising shows a moderate effect
* Newspaper advertising has weak or negligible influence

**Why this step is important:**
EDA helps guide model selection and provides early business insights.

---

### 2️⃣ Feature Selection & Train-Test Split

**Steps:**

* Selected TV, Radio, and Newspaper as input features
* Defined Sales as the target variable
* Split the dataset into training and testing sets

**Why this matters:**
Separating training and testing data ensures that model evaluation reflects real-world performance.

---

### 3️⃣ Baseline Model — Linear Regression

**Why Linear Regression?**

* Simple and highly interpretable
* Ideal baseline for comparison
* Easy to explain to business stakeholders

**Results:**

* Achieved high explanatory power (R² ≈ 0.9)
* Clearly showed that TV advertising is the main driver of sales

---

### 4️⃣ Model Evaluation & Visualization

**Evaluation Metrics:**

* R² Score
* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)

**Visualizations Used:**

* Actual vs Predicted Scatter Plot
* Residual Plot

**Purpose:**

* Validate model accuracy
* Detect underfitting or non-linear patterns

---

### 5️⃣ Regularization — Ridge & Lasso Regression

To address potential **multicollinearity** and improve model robustness, regularization techniques were applied.

#### 🔹 Ridge Regression

* Shrinks coefficients without eliminating features
* Improves stability and generalization

#### 🔹 Lasso Regression

* Performs automatic feature selection
* Identifies insignificant features

**Insight:**
Lasso regression confirmed that Newspaper advertising has minimal impact on sales.

---

### 6️⃣ Hyperparameter Tuning (Alpha Optimization)

**Approach:**

* Used GridSearchCV with cross-validation
* Tuned the `alpha` parameter for Ridge and Lasso models

**Why this step matters:**
Choosing the right alpha balances bias and variance, leading to better generalization.

---

### 7️⃣ Polynomial Regression

To explore non-linear relationships:

* Polynomial features (degree = 2) were introduced
* Linear Regression was applied on the expanded feature space

**Observation:**

* Slight improvement in performance
* Increased model complexity and reduced interpretability

**Decision:**
Polynomial regression should be used cautiously in business contexts.

---

### 8️⃣ Model Comparison Summary

| Model                 | Key Strength           | Limitation          |
| --------------------- | ---------------------- | ------------------- |
| Linear Regression     | Highly interpretable   | Linear assumptions  |
| Ridge (Tuned)         | Stable & robust        | Less sparse         |
| Lasso (Tuned)         | Feature selection      | Sensitive to alpha  |
| Polynomial Regression | Captures non-linearity | Harder to interpret |

---

## 📊 Final Results & Business Insights

* TV advertising consistently shows the highest impact on sales
* Regularization improves model reliability
* Lasso helps identify unnecessary features
* Simpler models provide strong business value

📌 **Business Recommendation:**

> Allocate a larger share of the advertising budget to TV while reassessing spending on Newspaper ads.

---

## ⚠️ Challenges Faced

* Multicollinearity between advertising channels
* Risk of overfitting with complex models
* Balancing accuracy with interpretability

### ✅ How We Addressed Them

* Applied Ridge & Lasso regularization
* Used cross-validation and tuning
* Preferred simpler, interpretable models

---

## 🎓 Lessons Learned

* Strong EDA leads to better modeling decisions
* Regularization is essential for regression problems
* More complex models are not always better
* Visualization is key to validating and explaining results

---

## 🧰 Tools & Technologies

* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn
* **Visualization:** Matplotlib, Seaborn
* **Deployment:** Streamlit

---

## 📊 Interactive Dashboard

A Streamlit dashboard was developed to:

* Compare regression models interactively
* Visualize actual vs predicted values
* Display feature importance dynamically

## 👤 Author

**Mohamed Ehab**  
Data Scientist | Machine Learning Engineer

- 📧 Email: moehab1532002@gmail.com  
- 📱 Phone: +20 109 014 6607  
- 🔗 LinkedIn: https://www.linkedin.com/in/mohamed-ehab-7b91092b3  
- 🐙 GitHub: https://github.com/Mohamedehabbb

⭐ *This project demonstrates a professional, end-to-end approach to regression modeling with a strong focus on business impact and interpretability.*


---

