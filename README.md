#  Titanic Dataset Analysis with Python & Pandas  

This project explores the **Titanic dataset** using Python and Pandas, focusing on data cleaning, feature engineering, aggregation, and visualization.  

---
![Titanic Age Distribution](images/plot-graph-titanic.png)

##  Project Workflow  

### 1. Exploratory Data Analysis (EDA)  
- Loaded the dataset and inspected its shape and summary statistics.  
- Identified missing values and calculated missing percentages.  

### 2. Feature Engineering  
- Created a new column:  
  ```python
  df["FamilySize"] = df["sibsp"] + df["parch"] + 1

## Added a categorical column FamilyCategory based on family size:
- Alone: FamilySize = 1
- Small: FamilySize = 2–4
- Large: FamilySize ≥ 5

## Data Cleaning
- Dropped high-missing-value columns: cabin, body, boat, home.dest.
- Cleaned dataset reduced from 14 columns → 9 columns.

## Sorting & Aggregation
- Sorted passengers by Age, Fare, and Class.
- Grouped by passenger class to calculate:
 
 | Passenger Class | Avg Fare | Survival Rate | Avg Age |
| --------------- | -------- | ------------- | ------- |
| 1st             | 87.51    | 0.62          | 37.81   |
| 2nd             | 21.18    | 0.43          | 29.42   |
| 3rd             | 13.31    | 0.26          | 25.75   |

## Data Visualization
- Visualized the distribution of ages.
- Plotted survival rates across classes.

## Key Insights
- 1st Class had the highest survival rate (~62%), while 3rd Class had the lowest (~25%).
- Younger passengers were more common in lower classes.
- Most passengers traveled alone or in small families.

## Tools Used
- Python
- Pandas
- Matplotlib (via Pandas .plot())
