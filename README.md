#  Student GPA Prediction 

This project builds a predictive system to estimate student GPA based on behavioral, academic, and demographic factors. It combines data analysis, model experimentation, and deployment into a single end-to-end workflow.

---

##  Problem Statement

Educational institutions often struggle to identify students who are at risk of underperforming.  
This project aims to:

- Predict student GPA using machine learning
- Identify key factors influencing academic performance
- Support early intervention strategies for at-risk students

---

##  Approach

The project follows a structured machine learning workflow:

1. **Exploratory Data Analysis (EDA)**
   - Understanding feature distributions and relationships
   - Identifying key drivers of GPA

2. **Feature Engineering**
   - Encoding categorical variables
   - Preparing data for modeling

3. **Model Development**
   - Baseline: Linear Regression
   - Ensemble: Random Forest

4. **Hyperparameter Tuning**
   - Optimization using Optuna

5. **Model Evaluation**
   - Regression metrics (MSE, R²)
   - Distribution comparison
   - Classification-based evaluation (GPA categories)


---

##  Results

| Model                  | MSE     | R²     |
|------------------------|---------|--------|
| Linear Regression      | 0.0386  | 0.9532 |
| Random Forest          | 0.0605  | 0.9268 |
| Tuned Random Forest    | 0.0591  | 0.9285 |

###  Key Insight
Despite using an ensemble model and hyperparameter tuning, **Linear Regression outperformed Random Forest**, indicating that the dataset has a strong linear structure.

This highlights an important lesson:
> Simpler models can outperform complex ones when the data is well-structured.

---

##  Business Insights

- **Attendance (Absences)** is the strongest negative factor affecting GPA  
- **Tutoring and structured activities** positively impact performance  
- **Behavioral factors** are more influential than demographics  
- The model effectively identifies **at-risk students (low GPA)**  

---

## Tech Stack

### Languages
- Python

### Libraries & Frameworks
- Pandas & NumPy → data processing
- Scikit-learn → modeling & pipeline
- Optuna → hyperparameter tuning
- Matplotlib & Seaborn → visualization
- Streamlit → deployment


