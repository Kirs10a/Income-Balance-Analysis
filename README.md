# Income-Balance-Analysis
This project involves analyzing a dataset using Python to extract meaningful insights about income, balance, and demographics, as per the requirements provided. The task demonstrates fundamental data handling and statistical analysis skills in Python, using libraries like pandas.

Project Overview
The purpose of this project is to load and analyze data from balance.txt using a Jupyter Notebook. The analysis answers specific questions related to income, balance, and demographics, providing insights into the dataset.

Key Objectives:
Compare the average income based on ethnicity.
Determine whether married or single individuals have a higher average balance.
Identify the highest and lowest income values in the dataset.
Count the number of recorded cards in the dataset.
Count the number of female and male records.
Dataset
The dataset is located in a file named balance.txt. It contains data on various individuals, including income, balance, marital status, gender, and ethnicity, which are essential for the required analysis.

Requirements
Python (version 3.6 or above)
Jupyter Notebook (for executing the .ipynb file)
Pandas (for data manipulation and analysis)
Ensure you have the required libraries installed. You can install pandas using:

bash
Copy code
pip install pandas
File Structure
bash
Copy code
├── Report.ipynb           # Jupyter Notebook file containing the data analysis code
├── balance.txt            # Dataset file
└── README.md              # Documentation file (you are currently reading)
Analysis Breakdown
1. Average Income by Ethnicity
The analysis calculates the average income for each ethnic group, providing insights into income distribution across different demographics.

2. Balance Comparison Based on Marital Status
This section compares the average balance for married and single individuals to see if there's a significant difference based on marital status.

3. Highest and Lowest Income in the Dataset
Identifies the maximum and minimum income values to understand the income range in the dataset.

4. Total Number of Cards
Calculates the total number of recorded cards in the dataset, giving a sense of the dataset’s size.

5. Gender Distribution
Counts the number of males and females in the dataset, offering insight into gender distribution.

Code Implementation
You can find the code in Report.ipynb. The code is structured as follows:

Data Loading: Loads the data from balance.txt into a pandas DataFrame.
Data Analysis: Uses pandas functions to perform statistical analysis as required:
groupby() for grouping data by ethnicity and marital status.
max() and min() for identifying highest and lowest incomes.
count() and sum() for counting records as needed.
Output: Each analysis is outputted directly in the notebook.
Example Code Snippets
Here are a few snippets to demonstrate the analysis.

Loading the Data:

python
import pandas as pd

# Load the data from balance.txt
df = pd.read_csv('balance.txt')
Average Income by Ethnicity:

python
avg_income_ethnicity = df.groupby('ethnicity')['income'].mean()
Comparison of Balance by Marital Status:

python
avg_balance_marital = df.groupby('marital_status')['balance'].mean()
Results
After running the code, the analysis provides answers to the key questions listed in the objectives section. The insights gained can help understand trends and disparities within the dataset.

Usage
To reproduce the analysis:

Open Report.ipynb in Jupyter Notebook.
Run each cell sequentially to load data, perform analysis, and generate results.
Contributing
Feel free to open a pull request or an issue if you want to contribute or have suggestions for improvement.
