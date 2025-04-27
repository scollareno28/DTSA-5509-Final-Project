# 💊 Drug Classification Using Supervised Machine Learning

## 📋 Project Overview

This project focuses on building predictive models to classify patients into appropriate drug treatments based on their health characteristics.  
Data was collected from patients suffering from the same illness, and each patient responded to one of five different medications.

Three supervised machine learning models were used:

- **Decision Tree Classifier**
- **Logistic Regression**
- **Random Forest Classifier**

The goal is to predict the appropriate drug for a new patient based on features such as age, sex, blood pressure, cholesterol levels, and sodium-to-potassium ratio (Na/K).

---

## 🛠️ Project Workflow

1. **Data Loading and Cleaning**
   - Imported and inspected the dataset (`drugdata200.csv`).
   - Cleaned categorical variables and rounded the Na/K ratio to two decimal places.
   - Mapped drug labels to simpler identifiers (A, B, C, X, Y).

2. **Exploratory Data Analysis (EDA)**
   - Visualized distributions of variables like Age, Sex, Blood Pressure, Cholesterol, and Na/K ratio.
   - Examined correlations (noted weak relationships between variables).
   - Explored how different features relate to drug classification.

3. **Data Preprocessing**
   - Label encoded categorical features.
   - Handled class imbalance by **undersampling** using `RandomUnderSampler`.

4. **Model Development**
   - Built and evaluated three models:
     - **Decision Tree**
     - **Logistic Regression**
     - **Random Forest**
   - Used classification reports and confusion matrices to assess performance.

5. **Model Comparison**
   - Random Forest achieved the highest accuracy and was the most robust across different drug classes.

6. **Model Improvement Attempts**
   - Experimented with hyperparameter tuning.
   - No significant improvements observed due to the nature of the dataset.

---

## 📊 Key Results

| Model                | Accuracy |
|----------------------|----------|
| Decision Tree        | 0.85     |
| Logistic Regression  | 0.70     |
| Random Forest        | 0.90     |

- **Random Forest** was the best performing model, achieving **90% accuracy**.
- **Logistic Regression** underperformed due to lack of strong linear relationships in the data.

---

## 📈 Future Improvements

- **Expand the dataset**: A larger dataset would improve model robustness and generalization.
- **Feature Engineering**: Incorporate additional health metrics if available.
- **Hyperparameter Tuning**: Further fine-tune models using grid search or random search.
- **Ensemble Methods**: Explore boosting algorithms like Gradient Boosting or XGBoost.
- **Cross-Validation**: Implement K-Fold Cross-Validation to validate model stability.

---

## 🧪 Technologies Used

- **Python 3.10+**
- **Pandas**, **NumPy** (Data manipulation)
- **Matplotlib**, **Seaborn** (Data visualization)
- **Scikit-learn** (Machine learning models, preprocessing)
- **Imbalanced-learn** (Handling imbalanced datasets)
- **Tabulate** (Result presentation)

