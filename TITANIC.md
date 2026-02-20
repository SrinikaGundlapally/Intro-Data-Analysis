# Titanic Dataset: Exploratory Data Analysis

## **Overview**
This project explores the Titanic dataset to see the key factors that played a part in passenger survival. Using Python, Pandas, Seaborn, and Matplotlib, I analyzed how demographics and social economic status played a role in the Titanic.

---

## **Objectives**
* **Perform Data Cleaning:** Handled missing values in `Age`, `Cabin`, and `Embarked`.
* **Feature Engineering:** Performed Encoding on categories like `Sex` and `Embarked` to prep them for mathematical analysis.
* **Visualization:** Created Heatmaps and Bar Plots to find hidden correlations between categorical variables.

---

## **Findings**
1. **Gender Bias:** Females had a higher survival rate than males, consistent with the "women and children first" policy.
2. **Class & Wealth:** The 1st Class who paid higher Fares were much more likely to survive compared to people in 3rd Class.
3. **Correlation:** There is a high negative correlation between **Pclass** and **Survival**, meaning as one goes to a lower status (class number goes up), survival chances go down.



---

## **Technologies Used**
* Python (Pandas, NumPy)
* Seaborn & Matplotlib for visualization
* Scikit-Learn for label encoding

---

## **How to Run**
1. Clone repository.
2. Open the `.ipynb` file in Jupyter Notebook or Kaggle.
3. Make sure you have the dataset `train.csv` in the same directory from Kaggle: https://www.kaggle.com/competitions/titanic
