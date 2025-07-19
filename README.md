# 🛡️ Credit Risk Classification - German Credit Dataset

This project presents an end-to-end credit risk modeling pipeline using the German Credit dataset. It aims to classify applicants into *good* or *bad* credit risk categories using various machine learning models, with a strong focus on recall to minimize false negatives in fraud/risk detection.

> 📍 Built using Python, Scikit-learn, Seaborn, and Plotly in Google Colab.

---

## 📊 Objectives

* Analyze key customer features contributing to credit risk.
* Handle class imbalance using oversampling.
* Train multiple classification models with cross-validation.
* Tune models for high recall — critical in risk-sensitive domains.
* Evaluate model performance using real-world metrics.

---

## 📁 Dataset

* **Source**: German Credit Risk Dataset
* **Target Variable**: `Risk` — binary classification (`good` / `bad`)
* **Key Features**:

  * Categorical: `Sex`, `Job`, `Housing`, `Saving accounts`, `Purpose`
  * Numerical: `Age`, `Credit amount`, `Duration`

---

## 🔍 Workflow Summary

### 1. 📥 Data Loading & Exploration

* Load data into pandas.
* Check for missing values, data types, and distributions.

### 2. 📊 EDA & Visualization

* Visualize feature distributions with respect to `Risk`.
* Analyze features like `Age`, `Credit Amount`, `Housing`, and `Purpose`.

### 3. ⚙️ Preprocessing

* One-hot encoding for categorical features.
* Oversampling to balance target classes.
* Standardization of numerical features.

### 4. 🤖 Model Training

* Train multiple models:

  * Logistic Regression
  * Linear Discriminant Analysis
  * KNN, Decision Tree, Naive Bayes
  * Random Forest, SVM
* Use **cross-validation with recall as scoring metric**

### 5. 🧪 Model Tuning

* Perform **GridSearchCV** on:

  * Random Forest
* Optimize for recall.

### 6. 📈 Final Evaluation

* Confusion Matrix
* Classification Report
* Accuracy, Recall, F-beta score

---

## 🧰 Tools & Libraries

* Python 3.10+
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn, Plotly
* Google Colab (hosted)

---

## ✅ Key Insights

* Class imbalance was significant (`bad risk` minority).
* Random Forest delivered best performance post-tuning.
* Oversampling + Scaling significantly improved recall.

---

## 📌 Future Work

* Deploy model via Streamlit dashboard.
* Add SHAP/ELI5 explainability for model transparency.
* Test pipeline on larger datasets with PySpark or Snowflake.
* Explore LLM (e.g., GPT-4) to auto-summarize key credit insights.



Let me know if you'd like a shortened version, or want it formatted for a GitHub README with badges or deployment options.
