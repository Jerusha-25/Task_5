# 🩺 Heart Disease Prediction using Decision Trees and Random Forests

## 📌 Objective
This project applies tree-based machine learning models (Decision Tree and Random Forest) to classify the presence of heart disease using patient data.

## 📊 Dataset
- **Source**: [Kaggle - Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
- **Features**: 13 medical attributes (age, sex, cp, trestbps, chol, etc.)
- **Target**: Presence of heart disease (0 = No, 1 = Yes)

---

## 🛠️ Tools & Libraries
- Python 3.x
- Pandas
- NumPy
- Matplotlib & Seaborn
- Scikit-learn
- Graphviz / `plot_tree` for visualization

---

## 🔍 Project Steps

### 1. Load and Explore Dataset
- Cleaned and explored the data for missing values and correlations.

### 2. Train Decision Tree Classifier
- Built an initial decision tree model.
- Visualized the full tree using `plot_tree`.

### 3. Analyze Overfitting
- Controlled overfitting using `max_depth` parameter.
- Compared training vs test accuracy.

### 4. Train Random Forest
- Trained a Random Forest classifier for better performance.
- Compared accuracy with the decision tree model.

### 5. Feature Importance
- Extracted and visualized top contributing features from the random forest model.

### 6. Cross-Validation
- Used 5-fold cross-validation to evaluate model stability.

---

## 📈 Results

| Model             | Train Accuracy | Test Accuracy | CV Accuracy |
|------------------|----------------|---------------|-------------|
| Decision Tree     | ~100% (unpruned) / ~84% (pruned) | ~80–85% | ~81% |
| Random Forest     | ~100%          | ~88–90%       | ~85–87%     |

✅ Random Forest outperforms Decision Tree in both accuracy and generalization.

---

## 📌 Conclusion
Tree-based models are effective for tabular datasets like this one. Random Forests help reduce overfitting and provide better accuracy. Feature importance analysis is also useful for interpretability in medical diagnosis contexts.




