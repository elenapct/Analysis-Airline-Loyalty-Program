# Flying Loyalty: Analysis of an Airline Loyalty Program

**Individual Project - Data Analytics Bootcamp (Adalab)** 🎓

This project is the result of my individual evaluation for Module 3 of the Adalab Data Analytics Bootcamp. The main goal was to conduct a comprehensive analysis of a customer loyalty program based on two original datasets:

- `Customer Flight Activity.csv`: Information about customers' flights.  
- `Customer Loyalty History.csv`: Information about customers and their participation in the loyalty program.

After cleaning, transforming, and merging the data, I created a unified dataset:

- `airline_loyalty_programme.csv`: Consolidated customer and flight information, ready for final analysis.

---

## Main tasks performed

- **Exploratory Data Analysis (EDA)**: understanding structure, unique values, and detecting duplicates.
- **Data Cleaning**: normalization of column names, data type adjustments, and consistency checks.
- **Handling Missing Values**: salary imputation using `IterativeImputer` and logical management of missing cancellation data.
- **Visualization and Insights Extraction**: graphical analysis to study customer behavior based on flights, points, geographic distribution, salaries, and loyalty card types.

---

## Challenges

Throughout this project, several challenges emerged that made the data analysis process particularly demanding:

- **Poor Data Quality**  
  Both original datasets contained a significant number of missing values and inconsistencies.

- **High Number of Duplicates**  
  In the flight dataset, many duplicate records were identified, not due to errors, but because the data was collected monthly for each customer, requiring a deeper understanding before deciding on aggregation strategies.

- **No Access to a Product Owner**  
  There was no direct stakeholder to clarify doubts or request missing information, forcing us to make critical assumptions based solely on the data exploration.

---

## Solutions

To address these challenges, the following strategies were implemented:

- **Understanding Duplicates**  
  Instead of removing apparent duplicates, I analyzed customer behavior across months and used `groupby().agg()` functions to appropriately consolidate data without losing information.

- **Missing Value Treatment**  
  For the `salary` column, I used an `IterativeImputer` strategy, selecting the most relevant features (`education`, `postal_code`) to improve the quality of the imputations and preserve logical consistency.

- **Clear Documentation of Assumptions**  
  Every assumption and decision made during the process (such as treating missing cancellation dates as active customers) was clearly documented to maintain transparency and reproducibility.

---

## Tools and Technologies

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Jupyter Notebook

------
------

Thanks for checking out this project!
Elena
