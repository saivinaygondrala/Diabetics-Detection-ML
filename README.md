# 🩺 Diabetics Detection using Machine Learning

This project aims to detect diabetes status (No Diabetes, Prediabetes, Diabetes) using health and lifestyle-related features. The entire workflow includes data preprocessing, visualization, model training, and performance comparison using different machine learning models.

---

## 📁 Dataset Description

- **File**: `diabetics.csv`
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/)
- **Target Variable**: `Diabetes_012`
  - `0`: No Diabetes  
  - `1`: Prediabetes  
  - `2`: Diabetes
- **Selected Features**:
  - HighBP, HighChol, CholCheck, BMI, Smoker, Stroke
  - HeartDiseaseorAttack, PhysActivity, HvyAlcoholConsump
  - AnyHealthcare, NoDocbcCost, GenHlth, MentHlth, PhysHlth
  - DiffWalk, Sex, Age

---

## 📊 Exploratory Data Analysis

Visualizations created to understand the data:
- Distribution of diabetes status
- Relationship between High Blood Pressure and Diabetes
- Diabetes proportions among smokers and age groups
- Correlation heatmap of features
- Pie chart of diabetes categories

Libraries used for visualization:
- `Matplotlib`
- `Seaborn`

---

## ⚙️ Machine Learning Models

### Preprocessing
- **Train-Test Split**: `80/20`, stratified by target
- **Feature Scaling**: `StandardScaler` from `sklearn`

### Models Trained
1. **Logistic Regression** (Baseline)
2. **Random Forest Classifier** with `class_weight='balanced'`
3. **XGBoost Classifier** (`multi:softmax`, 3-class output)

### Evaluation Metric
- **Accuracy Score**
- **Classification Report** from `sklearn.metrics`

---

## 🏆 Model Performance

| Model                | Accuracy     |
|---------------------|--------------|
| Logistic Regression | 84.53%       |
| Random Forest       | 79.30%       |
| XGBoost             | **84.80%**   |

> ✅ **XGBoost** achieved the best performance in terms of accuracy.

![Model Accuracy Comparison](<img width="855" height="557" alt="image" src="https://github.com/user-attachments/assets/7975203d-8066-477e-9e5d-a807a7291e03" />
)

---

## 📚 What I Learned

- Real-world health data preprocessing and feature selection
- Exploratory visualization using `Seaborn` and `Matplotlib`
- Multi-class classification using Logistic Regression, Random Forest, and XGBoost
- Comparing model performance using metrics and visual plots

---

## 🔧 Tools and Libraries Used

- `Python`
- `Pandas`, `NumPy`
- `Matplotlib`, `Seaborn`
- `Scikit-learn`
- `XGBoost`

---

## 📝 How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. Upload the `diabetics.csv` dataset.
3. Run the notebook cells sequentially to:
   - Preprocess data
   - Visualize insights
   - Train and evaluate models

---

## 📂 Project Structure

