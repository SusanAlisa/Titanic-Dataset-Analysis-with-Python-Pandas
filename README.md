#  Titanic Dataset Analysis with Python & Pandas  

This project explores the **Titanic dataset** using Python and Pandas, focusing on data cleaning, feature engineering, aggregation, and visualization.  

---

##  Project Workflow  

### 1. Exploratory Data Analysis (EDA)  
- Loaded the dataset and inspected its shape and summary statistics.  
- Identified missing values and calculated missing percentages.  

### 2. Feature Engineering  
- Created a new column:  
  ```python
  df["FamilySize"] = df["sibsp"] + df["parch"] + 1
