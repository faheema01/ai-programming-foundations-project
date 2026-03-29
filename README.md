NYC Airbnb 2019 — Data Analysis Project

Project Description:

This project performs exploratory data analysis (EDA) on the NYC Airbnb Open Data 2019 dataset.
It covers data cleaning, statistical summaries, grouped analysis, correlation checks, and three
Matplotlib/Seaborn visualizations to uncover pricing patterns across New York City boroughs and room types.

What I Built:

Two reusable data cleaning functions:
  - "remove_duplicates()" — detects and removes repeated rows
  - "normalize_column_names()" — standardises all column names to lowercase with underscores
- EDA functions (summary statistics, grouped analysis, correlation matrix, filtered views)
- Three visualizations: violin plot, grouped bar chart, and scatter plot with trend line


Name: NYC Airbnb Open Data 2019
Link: https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data

Data Cleaning and Bias Warning

Two cleaning functions were applied in this project:

- "remove_duplicates()" — removes repeated rows to prevent listings from
  being counted more than once, which would skew borough and price summaries.
  Confirmed zero duplicates in this dataset, but the check is documented as verified.

- "normalize_column_names()" — standardises all column names to lowercase
  with underscores, preventing silent KeyErrors in all downstream code.

Note: Missing values (10,052 in `last_review` and `reviews_per_month`) and
price outliers (up to $10,000) were not handled by a cleaning function. This means
price averages may be skewed by extremes, and review-based summaries reflect only
reviewed listings. These are acknowledged limitations for future improvement.





How to Run the Project:

1. Clone the repository
git clone [https://github.com/your-username/your-repo-name.git](https://github.com/faheema01/ai-programming-foundations-project.git)
cd ai-programming-foundations-project

2. Install dependencies
pip install -r requirements.txt

3. Open and run the notebook
jupyter notebook data_workflow.ipynb
Then select Kernel → Restart & Run All to execute all cells from top to bottom.

pip install -r requirements.txt

pip freeze > requirements.txt
