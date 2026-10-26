# Glassdoor-Market-Vizualization

Overview
This repository contains a data analysis and visualization project exploring the Data Science job market using a 2021 dataset scraped from Glassdoor. The project demonstrates a complete exploratory data analysis (EDA) pipeline, from initial data cleaning and preprocessing to generating visual insights regarding salaries, company ratings, and industry sectors.
Tech Stack
- Language: Python
- Data Manipulation: Pandas, NumPy
- Data Visualization: Matplotlib, Seaborn, Bokeh
- Environment: Jupyter Notebook

Data Cleaning & Preprocessing
To ensure accurate visualizations and insights, the raw dataset underwent rigorous preprocessing:
- Missing & Invalid Data Removal: Filtered out null placeholders (e.g., na job titles, -1 sectors, and -1.0 ratings).
- Dimensionality Reduction: Dropped irrelevant columns (like the unneeded index column) to streamline the dataset.
- Targeted Filtering: Removed vague job categories (e.g., 'other scientist') to focus strictly on core data science, analytics, and engineering roles.
- Data Standardization: Corrected text typos (e.g., standardizing 'data analitics' to 'data analytics').
- Feature Selection: Isolated the most impactful variables into a dedicated dataframe for analysis: Rating, Sector, Lower Salary, Upper Salary, Avg Salary(K), job_title_sim, and Degree.
- Outlier/Noise Reduction: Filtered the Sector column to only include industries with a statistically relevant number of job postings (count $\ge$ 5).

Visualizations & Insights
The notebook generates several key visualizations to answer business questions about the data science market:
1. Average Rating by Job Title: A bar chart ranking core data roles by their average company rating.
2. Average Rating by Industry Sector: A bar chart comparing how different sectors (Tech, Finance, Healthcare, etc.) score in employee satisfaction.
3. Salary vs. Rating (Scatter Plot): An exploratory plot observing the correlation (or lack thereof) between a company's Glassdoor rating and its average salary offerings.
4. Average Salary by Job Title: A comparative bar chart highlighting the most lucrative specific roles within the broader data science umbrella.

How to Run
1. Clone the repository to your local machine.
2. Ensure you have the required libraries installed (pip install pandas numpy matplotlib seaborn bokeh).
3. Update the CSV file path in the notebook to point to your local data directory.
4. Run the Jupyter Notebook cells sequentially.
