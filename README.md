# Student Performance Prediction

## 📌 Overview
This project aims to predict student academic performance (final grade - G3) based on various factors such as previous grades (G1, G2), study habits, family support, and other behavioral attributes. Using a **Linear Regression** model from scikit-learn, the project analyzes key features to forecast student outcomes with high accuracy (~89.6%).

## 🔍 Key Features
- **Data Preprocessing**: Handles categorical data (e.g., `famsup`) using `LabelEncoder`.
- **Feature Selection**: Focuses on impactful variables like:
  - Grades (G1, G2)
  - Absences, failures, study time, and free time.
  - Family support (`famsup`).
- **Model Training**: Uses `LinearRegression` with a **90-10 train-test split**.
- **Evaluation**: Achieves high accuracy (~0.896) and provides coefficient insights.

## 📊 Results
- **Accuracy**: **89.6%** (R² score).
- **Key Predictors**:
  - **G2 (previous grade)** has the highest coefficient (`0.98`), indicating strong correlation with G3.
  - **Absences** and **failures** negatively impact performance (`-0.32` and `-0.23` coefficients).
  - **Family support** (`famsup`) shows a positive effect (`0.23`).

## 🛠️ Tools & Libraries
- **Python**: Primary programming language.
- **Pandas & NumPy**: Data manipulation.
- **Scikit-learn**: Machine learning (`LinearRegression`, `LabelEncoder`, `train_test_split`).
- **Matplotlib/Seaborn**: Visualization (not shown but suggested for EDA).

## 📂 Dataset
- **Source**: `student-mat.csv` (UCI ML Repository-style data).
- **Columns Used**:  
  `G1`, `G2`, `G3`, `absences`, `failures`, `studytime`, `freetime`, `famsup`.

## 🎯 Potential Applications
- **Educators**: Identify at-risk students early.
- **Policy Makers**: Design interventions based on key predictors (e.g., reducing absences).
- **Students**: Self-assess performance trends.

## 🔧 How to Run
1. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
2. Clone the repository and run the Jupyter notebook.

## 📈 Future Work
- Include more features (e.g., socio-economic factors).
- Try advanced models (Random Forest, Gradient Boosting).
- Add visualizations for EDA and results.

---

**Tags**: `#Education` `#MachineLearning` `#LinearRegression` `#Python` `#DataScience`
