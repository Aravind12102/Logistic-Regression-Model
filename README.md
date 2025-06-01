# Logistic-Regression-Model

This project uses **Logistic Regression** to perform binary classification on the **Breast Cancer Wisconsin dataset**. The objective is to accurately classify tumors as either **Malignant (M)** or **Benign (B)** based on various medical imaging features.

---

##  Dataset

- **Source**: Breast Cancer Wisconsin (Diagnostic) Dataset
- **Total Instances**: 569
- **Features**: 30 numeric features (mean, SE, and worst of measurements like radius, texture, perimeter, area, etc.)
- **Target Variable**: `diagnosis` — `'M'` (Malignant) or `'B'` (Benign)

---

##  Tools & Libraries

- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

---

## Steps Performed

### 1. Data Preprocessing
- Dropped unnecessary columns: `id`, `Unnamed: 32`
- Encoded target labels: `'M'` → `1`, `'B'` → `0`
- Split dataset into training (80%) and testing (20%) sets
- Standardized features using `StandardScaler`

### 2. Model Training
- Used **Logistic Regression** with `scikit-learn`
- Trained on scaled data with `max_iter=10000`

### 3. Model Evaluation
- **Confusion Matrix**
- **Classification Report**: precision, recall, F1-score
- **ROC-AUC Score** and **ROC Curve**
- **Threshold Tuning**: Visualized precision and recall vs threshold

### 4. Sigmoid Function Explanation
- Demonstrated how Logistic Regression uses the sigmoid function:
  \[
  \sigma(z) = \frac{1}{1 + e^{-z}}
  \]
- Visualized sigmoid curve

---

## Results

- **Accuracy**: ~97%
- **ROC-AUC Score**: ~0.997
- Logistic Regression showed excellent classification performance.

---

