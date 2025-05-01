# 📊 Bank Marketing Classification with Decision Tree and AdaBoost

This project applies machine learning classification techniques on the [Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing). We first use a **Decision Tree Classifier** and then enhance the model's performance with **AdaBoost**, a powerful ensemble learning method.

---

## 📁 Dataset

**File Used**: `bank.csv`  
This dataset contains marketing data related to direct telemarketing campaigns of a Portuguese banking institution. The goal is to predict whether a client will subscribe to a term deposit (`y` column).

---

## ✅ Project Workflow

1. **Data Preprocessing**
   - Handle categorical and numerical features
   - One-hot encoding of categorical variables
   - Train-test split

2. **Model 1: Decision Tree Classifier**
   - Baseline model
   - Evaluated using accuracy, precision, recall, F1-score

3. **Model 2: AdaBoost Classifier**
   - Uses the decision tree as the base estimator
   - Boosts accuracy by combining multiple weak learners
   - Performance compared against the baseline model

---

## 🛠️ Dependencies

Install required libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## 🚀 How to Run

```bash
python main.py
```

Your script should:
- Load and preprocess `bank.csv`
- Train and evaluate the decision tree
- Train and evaluate AdaBoost
- Print performance metrics for both

---

## 📈 Results Snapshot (Example)

| Model                | Accuracy | Precision | Recall | F1 Score |
|---------------------|----------|-----------|--------|----------|
| Decision Tree        | 0.87     | 0.73      | 0.65   | 0.69     |
| AdaBoost Classifier  | 0.90     | 0.80      | 0.72   | 0.76     |

---

## 📌 Notes

- Feature importance can be visualized for both models.
- You can tweak AdaBoost parameters like `n_estimators` and `learning_rate` for tuning.
- Ensure reproducibility by setting random seeds.

---

## 📚 References

- [UCI Machine Learning Repository - Bank Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)
- [Scikit-learn: Decision Trees](https://scikit-learn.org/stable/modules/tree.html)
- [Scikit-learn: AdaBoost](https://scikit-learn.org/stable/modules/ensemble.html#adaboost)
