# Titanic Survival Prediction

This project uses the Titanic dataset to predict passenger survival using machine learning techniques. It involves data cleaning, feature engineering, model building, and evaluation using classification algorithms like Random Forest.

---

## 📊 Dataset

- Source: Kaggle Titanic Dataset
- Features: Name, Age, Gender, Pclass, Fare, Embarked, SibSp, Parch, etc.
- Target: `Survived` (0 = No, 1 = Yes)

---

## 🎯 Objectives

- Explore and clean the data
- Visualize relationships (e.g., gender vs. survival)
- Train classification models (Logistic Regression, Random Forest)
- Evaluate and compare model performance
- Derive insights for survival trends

---

## 🛠️ Tools & Technologies

- **Programming**: Python
- **Libraries**: pandas, numpy, seaborn, matplotlib, scikit-learn
- **Environment**: Jupyter Notebook
- **Model**: RandomForestClassifier
- **Metric**: Accuracy Score

---

## 🔍 Key Questions Addressed

1. What was the overall survival rate?
2. Did gender or passenger class affect survival?
3. How did age distribution differ between survivors and non-survivors?
4. Can we predict survival using machine learning?

---

## 📈 Main Findings

1. **Overall Survival Rate**
   - 38.38% of passengers survived.
   - Visualized with a countplot showing 549 non-survivors and 342 survivors.

2. **Impact of Gender and Passenger Class**
   - Female passengers had significantly higher survival rates.
   - 1st-class passengers had the highest survival (~65%).
   - A clear survival advantage was found for females and upper classes.

3. **Age Distribution**
   - Children (<10 years) had higher survival rates.
   - Most non-survivors were aged 20–40.
   - KDE plot showed distinct age trends between survivors and non-survivors.

4. **Modeling**
   - RandomForestClassifier was used for predictions.
   - Achieved 82% accuracy on the test set.

---

## 🧹 Data Cleaning Summary

- **Missing Values**:
  - Age: filled with median
  - Embarked: filled with mode
- **Dropped Irrelevant Columns**:
  - PassengerId, Name, Ticket, Cabin
- **Categorical Encoding**:
  - Sex: male = 0, female = 1
  - Embarked: S = 0, C = 1, Q = 2

---

## 💡 Key Insights

- "Women and children first" was evident in survival rates.
- 1st-class passengers were prioritized during rescue.
- Gender and class were critical predictors.
- Family size (SibSp + Parch) has potential for deeper analysis.

---

## ✅ Recommendations

- Always include gender and class in survival prediction models.
- Consider engineering features like family size or fare-per-person.
- Visualizations should support every key step in analysis.

