# EDAtask8 – Student Performance Analysis

## Project Overview

This project performs Exploratory Data Analysis (EDA) on the **StudentsPerformance.csv** dataset. It explores students' mathematics, reading, and writing scores, checks data quality, standardizes categorical values, calculates statistical measures, creates total marks and percentage columns, identifies outliers, and visualizes score patterns across student groups.

## Objectives

- Understand the structure and quality of the dataset.
- Check for missing values and duplicate records.
- Clean and standardize categorical columns.
- Calculate mean, median, standard deviation, and quartiles.
- Create `total marks` and `percentage` columns.
- Detect score outliers using the Interquartile Range (IQR) method.
- Compare scores by parental education, lunch type, and test preparation status.
- Explore relationships and correlations among subject scores.

## Dataset

**File:** `StudentsPerformance.csv`

The dataset contains **1,000 student records** and **8 original columns**.

| Column | Description |
|---|---|
| `gender` | Student gender |
| `race/ethnicity` | Student group |
| `parental level of education` | Parent's education level |
| `lunch` | Lunch category |
| `test preparation course` | Test preparation status |
| `math score` | Mathematics score |
| `reading score` | Reading score |
| `writing score` | Writing score |

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## Project Workflow

1. **Import libraries** – Load Pandas, NumPy, Matplotlib, and Seaborn.
2. **Load the dataset** – Read `StudentsPerformance.csv` into a Pandas DataFrame.
3. **Inspect the data** – Display the first five rows, dataset shape, and data types.
4. **Check data quality** – Identify missing values and duplicate records.
5. **Descriptive statistics** – Review count, mean, standard deviation, minimum, quartiles, and maximum.
6. **Clean categorical columns** – Convert categorical values to string type, remove extra spaces, and change text to lowercase.
7. **Calculate statistics** – Find mean, median, standard deviation, and Q1, Q2, and Q3 for each subject.
8. **Create new features** – Calculate total marks out of 300 and percentage.
9. **Detect outliers** – Apply the IQR method to math, reading, and writing scores.
10. **Visualize the data** – Compare subject scores and examine relationships using charts.
11. **Export the result** – Save the processed dataset as `Student_Performance_Cleaned.csv`.

## Visualizations

The notebook creates the following visualizations:

- Bar chart: Average scores by parental education level.
- Bar chart: Average scores by lunch type.
- Box plots: Math, reading, and writing scores by test preparation status.
- Scatter plots: Math vs. reading, math vs. writing, and reading vs. writing scores.
- Correlation heatmap: Correlation among the three subject scores.

## Key Findings

- The dataset contains **1,000 rows** and **8 original columns**.
- No missing values were found.
- No duplicate records were found.
- Average subject scores:
  - Math: **66.09**
  - Reading: **69.17**
  - Writing: **68.05**
- Average total marks: **203.312 out of 300**.
- Average percentage: **67.7707%**.
- IQR outlier counts:
  - Math: **8**
  - Reading: **6**
  - Writing: **5**

The visualizations help compare student scores across parental education and lunch categories, examine score distributions by test preparation status, and understand relationships among the three subjects.

## How to Run the Project

### 1. Clone or download the project

Download this repository to your computer.

### 2. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Place the dataset

Keep `StudentsPerformance.csv` in the project folder, or update the CSV path in the notebook to match its location.

### 4. Open the notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open `EDA task8.ipynb` and run the cells in order.

**Google Colab:** Upload `StudentsPerformance.csv` to the Colab session and make sure the notebook's CSV path points to the uploaded file.

## Output

After running the notebook, the processed dataset is saved as:

```text
Student_Performance_Cleaned.csv
```

This file includes the original columns along with the calculated `total marks` and `percentage` columns.

## Project Structure

```text
EDA-Student-Performance/
├── EDA task8.ipynb
├── StudentsPerformance.csv
├── Student_Performance_Cleaned.csv
├── README.md
└── images/
    ├── parental_education_scores.png
    ├── lunch_scores.png
    ├── math_test_prep.png
    ├── reading_test_prep.png
    ├── writing_test_prep.png
    ├── math_reading_scatter.png
    ├── math_writing_scatter.png
    ├── reading_writing_scatter.png
    └── score_correlation_heatmap.png
```

*Note: The CSV output and image files are generated or saved when the corresponding notebook cells are run. Add them to the repository if you want them included in the project structure.*

## Conclusion

This project explores student performance in mathematics, reading, and writing through data inspection, cleaning, statistical analysis, feature creation, outlier detection, and visualization. The analysis provides a clear overview of score distributions and how student performance varies across selected categories.

---

**Author:** WILSON JEBASEELAN J  
**Task:** EDA Task 8 – Exploratory Data Analysis  
**Dataset:** StudentsPerformance.csv
