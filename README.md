# 🔐 Logistic Regression Project – A Complete Walkthrough

This project explores **Logistic Regression** in depth by applying it to multiple types of classification problems. It covers binary classification, multiclass classification, imbalanced data handling, and ROC-AUC evaluation, along with performance improvements using **hyperparameter tuning** and **cross-validation** techniques.

---

## 📌 Project Overview

The project is divided into **four parts**, each addressing a unique use case of Logistic Regression:

1. **Binary Classification using synthetic dataset**
2. **Multiclass Classification**
3. **Imbalanced Classification**
4. **ROC Curve & AUC Evaluation**

For each case, the model is built, trained, evaluated, and tuned for better performance.

---

## 🧪 Part 1: Binary Classification

- 📊 **Dataset:** Created using `make_classification` with 1000 samples, 10 features, and 2 classes
- ⚙️ **Model:** Logistic Regression
- 📈 **Predictions:** Both class labels and probability predictions
- 📊 **Evaluation:**
  - Accuracy Score
  - Confusion Matrix
  - Classification Report
- 🧠 **Model Improvement:**
  - Performed **GridSearchCV** to find best parameters and score
  - Also used **RandomizedSearchCV** for faster, randomized parameter tuning
  - Re-evaluated using performance metrics after tuning

---

## 🧪 Part 2: Multiclass Classification

- 📊 **Dataset:** Created with 1000 samples, 10 features, and **3 classes**
- 🔄 **Model:** Multinomial Logistic Regression
- 📈 **Result:** Achieved around **79% accuracy**
- 🚀 **Next Step:** Model can be further improved using hyperparameter tuning techniques

---

## ⚖️ Part 3: Imbalanced Classification

- 📊 **Dataset:** Created with 1000 samples, **2 features**, and class weights of `0.99` (high imbalance)
- 📌 **Visualization:** Scatter plot showed extreme class imbalance
- 🛠️ **Handling:**
  - Applied `class_weight='balanced'` in Logistic Regression
  - Used **GridSearchCV** to optimize parameters
- ✅ **Result:** Achieved **99% accuracy**, showing significant improvement after handling imbalance

---

## 📈 Part 4: ROC Curve and AUC Score

- ⚙️ **Setup:**
  - Created a dummy model (always predicts 0) for baseline
  - Trained Logistic Regression and generated probability predictions
- 📊 **Evaluation:**
  - Calculated **FPR** (False Positive Rate) and **TPR** (True Positive Rate)
  - Plotted **ROC Curve**
  - Computed **ROC AUC Score**
- 🔍 **Threshold Tuning:**
  - Learned how to select classification thresholds using ROC curve insights

---

## 📊 Techniques Used

| Technique / Tool     | Purpose                                |
|----------------------|----------------------------------------|
| `make_classification`| Synthetic dataset generation           |
| Logistic Regression  | Core classification model              |
| GridSearchCV         | Hyperparameter tuning (exhaustive)     |
| RandomizedSearchCV   | Hyperparameter tuning (randomized)     |
| ROC, AUC             | Classification threshold and score eval|
| `matplotlib`, `seaborn` | Visualization and plots             |
| `scikit-learn`       | Models, metrics, and dataset generation|

---

## 🗂️ Project Structure

| File Name                           | Description                                  |
|------------------------------------|----------------------------------------------|
| `Logistic Regression.ipynb` | Classification | 
| `README.md`                        | Project overview and documentation (this)    |

---

## 🚀 Getting Started

1. **Clone the Repository**

   ```bash
   git clone https://github.com/YourUsername/Logistic-Regression-Project.git
   cd Logistic-Regression-Project

2. **Install required libraries**

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn

3. **Launch Jupyter Notebook**

   ```bash
   jupyter notebook

4. **Open ipynb files and run through the cells.**

| Scenario                  | Dataset Type  | Accuracy | Key Improvement         |
| ------------------------- | ------------- | -------- | ----------------------- |
| Binary Classification     | Balanced      | High     | Grid & Random SearchCV  |
| Multiclass Classification | 3 Classes     | \~79%    | Can be improved further |
| Imbalanced Classification | Skewed (0.99) | \~99%    | Class weight + tuning   |
| ROC Curve Analysis        | Binary        | —        | Threshold selection     |


👩‍💻 Author
Maitri Prabhu
GitHub: Mai3Prabhu
