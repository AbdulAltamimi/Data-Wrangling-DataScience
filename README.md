Data Science Job Market Analysis
A comprehensive data wrangling and analysis project examining data science job salaries and market demand using real-world datasets.
Project Overview
This project applies data gathering, assessment, cleaning, and analysis techniques to explore two key questions in the data science job market:

Which data science job titles command the highest salaries in USD?
What are the top 10 most in-demand data science positions?

Datasets
Dataset 1: Data Science Salaries

Source: Hugging Face (hugginglearners/data-science-job-salaries)
Method: Programmatic download
Size: 500+ records
Key Variables:

Work year, experience level, employment type
Job title, salary (USD)
Employee residence, remote ratio
Company location and size



Dataset 2: Glassdoor Jobs

Source: Kaggle
Method: Manual download
Size: 500+ records
Key Variables:

Job title, salary estimates (min/max)
Job description, company rating
Company name, location, size
Industry, sector, revenue



Data Quality Issues Addressed
Quality Issues

Completeness: Handled 375+ missing salary values, 270+ missing ratings, and other null values
Duplicates: Removed 680 duplicate records from the jobs dataset

Tidiness Issues

Column Structure: Split salary estimates into separate min_salary and max_salary columns
Redundancy: Removed unnecessary columns (salary, salary_currency, Unnamed: 0) to maintain single standardized salary representation

Project Structure
├── raw data/
│   ├── salary_raw.csv
│   └── jobs_raw.csv
├── cleaned data/
│   ├── salary_clean_data_cleaned.csv
│   ├── jobs_clean_data_cleaned.csv
│   └── combined_data_cleaned.csv
└── analysis.ipynb
Key Findings
Highest Paying Role
<img width="1244" height="1107" alt="stat" src="https://github.com/user-attachments/assets/d78c7d31-7200-458a-9e0a-6a5228461d48" />
Data Analytics Lead emerged as the highest-paying job title in the data science field based on average salary analysis.
Most In-Demand Position
<img width="902" height="712" alt="image" src="https://github.com/user-attachments/assets/5366671a-f29e-47f8-a22b-90b4cf8b6f3b" />

Data Scientist is the most frequently listed position, significantly outpacing other roles in job market demand.
Data Cleaning Pipeline

Assessment: Visual and programmatic inspection of data quality
Cleaning:

Replace placeholder values (-1) with NaN
Drop null values and duplicates
Split composite columns
Remove redundant variables


Storage: Save both raw and cleaned versions
Combination: Merge relevant features from both datasets

Future Improvements
With additional time, this project could be enhanced by:

Deeper analysis of salary disparities by location and experience level
Trend analysis across different years
Geographic clustering of job opportunities
Predictive modeling for salary estimation
Industry-specific salary comparisons
