# Employee Attendance Analysis with PySpark

# 

### This project analyzes employee attendance and salary data using PySpark. The goal is to compute effective salaries based on attendance percentage and derive department-wise insights.

### 

#### 📁 Project Structure



##### employee-attendance-analysis/

##### │

##### ├── attendance\_big.xlsx # Raw attendance data

##### ├── employees\_big.xlsx # Raw employee data

##### ├── employee\_analysis.ipynb # Main analysis code in Jupyter Notebook

##### ├── README.md # Project overview and instructions





#### 📊 Data Description



##### 1\. `employees\_big.xlsx`

###### Contains employee details:

###### \- `employee\_id`

###### \- `name`

###### \- `department`

###### \- `salary`

###### 

##### 2\. `attendance\_big.xlsx`

###### Contains daily attendance logs:

###### \- `employee\_id`

###### \- `attendance\_date`

###### \- `status` (e.g., Present, Absent, NA)

###### 

##### ✅ Tasks Performed

###### 

###### \- Imputed missing salaries using \*\*department-wise median\*\*

###### \- Cleaned and standardized attendance status

###### \- Calculated:

###### &nbsp; - Monthly attendance percentage

###### &nbsp; - Effective salary (based on actual presence)

###### \- Aggregated metrics at \*\*department level\*\*

##### 

##### 💡 Final Output

###### 

###### \- Average attendance percentage per department

###### \- Total effective salary per department

##### 

##### 🛠️ Technologies Used

###### 

###### \- Apache Spark (PySpark)

###### \- Python

###### \- Jupyter Notebook

###### \- Excel/CSV for raw data

###### 

##### 🚀 How to Run

###### 

###### 1\. Open the notebook `employee\_analysis.ipynb` in Jupyter

###### 2\. Make sure PySpark is installed and running

###### 3\. Replace the file paths if necessary

###### 4\. Run all cells to perform analysis



#### 

#### Notes

\- Missing or invalid attendance status (e.g., NA, null, blank) is treated as \*\*Absent\*\*

\- Salary is filled using \*\*`percentile\_approx()`\*\* for department-wise median

\- Analysis assumes working days = days with any attendance record



---





