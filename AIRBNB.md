# Airbnb Data Analysis
**Project:** Data Cleaning and Insight Generation from Survey Data  
**Dataset:** Airbnb Open Data (New York City)

---

## Task Description
This project worked on Data Cleaning and Insight Generation. It demonstrates the ability to handle real-world data and extract meaningful behavioral insights.

### Topics:
* **Data Cleaning:**
    * Removed inconsistent formatting in `price` and `service_fee` columns.
    * Handled missing values and duplicates.
* **Categorical Handling:**
    * Applied Label Encoding for nominal data (Neighbourhood Groups).
* **Insight Generation:**
    * Extracted insights regarding respondent behavior and preferences.

---

## Implementation

**Tools Used:** Python, Pandas, Seaborn, Matplotlib, Scikit-Learn.

**How to Run:** Ensure you have the dataset from Kaggle: Airbnb Open Data https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata

The final cleaned dataset will be exported as cleaned_airbnb_data.csv.


## Insights Summary

The summary dashboard highlights the most expensive neighborhoods, demonstrating host pricing behavior and guest preferences in the NYC market.

### Data Cleaning
The dataset contained prices as strings (e.g., `"$966 "`). I used the following logic to convert them to integers:
```python
data['price'] = data['price'].astype(str).str.replace('$', '').str.replace(',', '').str.strip()
data['price'] = pd.to_numeric(data['price'], errors='coerce').fillna(0).astype(int)
