# Boston Housing Price Prediction: SLR, MLR, and Polynomial Regression

This project explores the use of different regression techniques — Simple Linear Regression (SLR), Multiple Linear Regression (MLR), and Polynomial Regression — to predict house prices using the **Boston Housing** dataset. The workflow includes data preprocessing, correlation analysis, model training, and evaluation.

---

## 📁 Contents

- `boston_regression_models.ipynb`: Main notebook containing the full code, analysis, and visualizations.
- `README.md`: Project overview and methodology.

---

## 🧹 Data Preprocessing

1. **Dataset Used**:  
   - Boston Housing dataset from `kaggle`.

2. **Handling Missing Values**:  
   - Verified the dataset contains no missing values.

3. **Feature Names & Description**:  
   - The dataset contains 13 numerical features like average number of rooms, crime rate, distance to employment centers, etc.

4. **Train-Test Split**:  
   - Data was split into training (80%) and test (20%) sets using `train_test_split`.

---

## 🔍 Correlation Analysis

- A **correlation matrix** and **heatmap** were created to understand relationships between features and the target (`MEDV` - median house value).
- Highly correlated features were used for SLR and MLR.
- Correlation analysis helped avoid multicollinearity and informed better feature selection.

---

## 🧮 Models Implemented

### ✅ 1. Simple Linear Regression (SLR)
- Used a single feature (`LSTAT`) most correlated with `MEDV`.
- Established a baseline model.

### ✅ 2. Multiple Linear Regression (MLR)
- Included multiple features based on correlation and domain knowledge.
- Improved performance and captured more complex relationships.

### ✅ 3. Polynomial Regression
- Extended linear regression by including polynomial terms (degree 3).
- Captured non-linear relationships in the data.

---

## 📊 Evaluation Metrics & Visual Diagnostics

- **R² Score** and **MSE** used for model comparison.
- **Residual Plots**: Checked for randomness (no pattern = good).

---

## 📚 Tools & Libraries

- Python 3
- `pandas`, `numpy`
- `scikit-learn`
- `seaborn`, `matplotlib`

---

## 📌 Key Insights

- `LSTAT` had the strongest negative correlation with house price.
- Polynomial Regression (degree 3) outperformed SLR and MLR for non-linear patterns.
- Overfitting became noticeable with higher-degree polynomials.

---

## 🏷️ License

This project is open-source and available under the MIT License.

---

## 📎 Dataset Acknowledgment

Boston Housing Dataset © UCI/StatLib, redistributed via **Kaggle**, CC0 Public Domain :contentReference[oaicite:2]{index=2}.
