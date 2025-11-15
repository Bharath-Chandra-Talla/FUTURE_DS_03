# 📊 Student Feedback Survey Analysis

## Project Overview

This project analyzes student feedback survey responses to quantitatively assess overall satisfaction and identify specific strengths and weaknesses in course delivery and student support. The analysis utilizes core data science techniques to transform raw rating data into clear, actionable business insights.

### Files in Repository

| File Name | Description |
| :--- | :--- |
| **`Student_Feedback_Analysis.ipynb`** | The main Jupyter Notebook containing all the code, methodology, data cleaning steps, statistical analysis, and final conclusions. |
| **`student_feedback.csv`** | The raw, anonymized dataset (1001 entries) containing student ratings (scores from 1 to 10) across eight course aspects. |
| **`Outputs`** | It contains images of the dashboard|

## Methodology & Analysis Steps

The analysis was performed using Python (Pandas/NumPy) and involved the following steps:

1.  **Data Preparation:** The raw rating columns were cleaned and prepared for numerical analysis.
2.  **Feature Engineering:** An **`Overall Rating`** was calculated for each student by taking the average of all individual rating scores.
3.  **Satisfaction Classification:** Each student was categorized into one of three groups based on their `Overall Rating`:
    * **Satisfied** (Rating > 7)
    * **Neutral** (Rating 5 - 7)
    * **Dissatisfied** (Rating < 5)
4.  **Key Metric Calculation:** Mean scores for all eight course aspects were computed to rank performance.

## Key Project Findings

The analysis successfully quantified student perception, revealing crucial areas for strategic focus:

| Finding | Detail |
| :--- | :--- |
| **Dominant Sentiment** | **70.0%** of students were classified as **Neutral**, highlighting a major opportunity to improve overall satisfaction by converting this large segment. |
| **Top Strength** | The highest-rated area was **Faculty Subject Knowledge** (Average Score: **~7.5**). |
| **Critical Focus Areas** | The lowest-rated metrics identified as needing immediate improvement were **Degree of difficulty of assignments** and **Solves doubts willingly** (Average Scores: **~5.4-5.5**). |


## 🛠️ Tools and Libraries Used

The analysis that generated these visuals was conducted using the following primary tools and Python libraries:

| Tool/Library | Purpose in Project |
| :--- | :--- |
| **Python** | The core programming language used for scripting and executing the analysis. |
| **Pandas** | Essential for loading the CSV data, cleaning it, performing numerical calculations (like the `Overall Rating` average), and data manipulation. |
| **NumPy** | Used for efficient mathematical operations, particularly array manipulation and calculation of means and statistics. |
| **Matplotlib** | Used to create static, embeddable visualizations (charts, plots) for presentation of the key findings. |
| **Seaborn** | Used to create aesthetically pleasing and informative statistical graphics, often used to visualize distributions and relationships in the data. |

---

## How to Run the Analysis

To reproduce the analysis and generate the final output file (`student_feedback_with_insights.csv`):

1.  **Clone the Repository:** Download the files to your local machine.
2.  **Install Dependencies:** Ensure you have the necessary libraries installed (e.g., `pandas`, `numpy`).
3.  **Run the Notebook:** Open and run all cells in the **`Student_Feedback_Analysis.ipynb`** notebook.

The notebook will automatically load the CSV, perform the analysis, and save the final dataset with the added insight columns.
