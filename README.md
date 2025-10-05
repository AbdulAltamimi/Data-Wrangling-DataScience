# 💼 Data Science Job Market Analysis

A comprehensive **data wrangling and analysis project** examining **data science job salaries and market demand** using real-world datasets from **Hugging Face** and **Kaggle**.

---

## 📘 Project Overview

This project applies **data gathering, assessment, cleaning, and analysis** techniques to explore two key questions in the data science job market:

1. **Which data science job titles command the highest salaries (in USD)?**  
2. **What are the top 10 most in-demand data science positions?**

By combining and cleaning datasets from different sources, the project provides a clear picture of both **salary trends** and **job market demand** in the data science field.

---

## 🧾 Datasets

### 🧠 Dataset 1: Data Science Salaries
- **Source:** [Hugging Face – hugginglearners/data-science-job-salaries](https://huggingface.co/datasets/hugginglearners/data-science-job-salaries)  
- **Method:** Programmatic download  
- **Size:** 500+ records  
- **Key Variables:**
  - `work_year`, `experience_level`, `employment_type`
  - `job_title`, `salary_in_usd`
  - `employee_residence`, `remote_ratio`
  - `company_location`, `company_size`

### 🏢 Dataset 2: Glassdoor Jobs
- **Source:** [Kaggle](https://www.kaggle.com/)  
- **Method:** Manual download  
- **Size:** 500+ records  
- **Key Variables:**
  - `Job Title`, `Salary Estimate (min/max)`
  - `Job Description`, `Rating`
  - `Company Name`, `Location`, `Size`
  - `Industry`, `Sector`, `Revenue`

---

## 🧹 Data Quality & Tidiness Issues Addressed

### 🔧 Quality Issues
- **Missing Values:**  
  - 375+ missing salary estimates  
  - 270+ missing company ratings  
  - 471+ missing founded years  
  - 309+ missing industry/sector entries  
- **Duplicates:**  
  - Removed **680 duplicate records** from the Glassdoor dataset.

### 🧩 Tidiness Issues
- **Column Structure:**  
  - Split `Salary Estimate` into separate `min_salary` and `max_salary` columns.  
- **Redundant Data:**  
  - Removed unnecessary columns such as `salary`, `salary_currency`, and `Unnamed: 0` to maintain a single standardized salary representation (`salary_in_usd`).

---
## 📈 Key Findings

### 💰 Highest Paying Role
<img width="1244" height="1107" alt="stat" src="https://github.com/user-attachments/assets/d78c7d31-7200-458a-9e0a-6a5228461d48" />

**Data Analytics Lead** emerged as the **highest-paying job title** in the data science field based on average salary analysis.

---

### 🔍 Most In-Demand Position
<img width="902" height="712" alt="image" src="https://github.com/user-attachments/assets/5366671a-f29e-47f8-a22b-90b4cf8b6f3b" />

**Data Scientist** is the **most frequently listed position**, significantly outpacing other roles in job market demand.

---

## 🧰 Data Cleaning Pipeline

1. **Assessment:**  
   - Inspected data visually and programmatically to detect missing values, duplicates, and column inconsistencies.  
2. **Cleaning:**  
   - Replaced placeholder values (`-1`) with `NaN`.  
   - Dropped missing and duplicate records.  
   - Split composite columns (e.g., `Salary Estimate` → `min_salary`, `max_salary`).  
   - Removed redundant variables.  
3. **Storage:**  
   - Saved both **raw** and **cleaned** versions for reproducibility.  
4. **Combination:**  
   - Merged relevant variables from both datasets for joint analysis.

---

## 🚀 Future Improvements

With additional time and resources, this project could be expanded to include:

- **Deeper Salary Analysis:** Explore disparities by **location**, **experience level**, and **employment type**.  
- **Temporal Trends:** Analyze salary and demand changes **across years**.  
- **Geographic Insights:** Cluster opportunities by **region or country**.  
- **Predictive Modeling:** Build ML models to estimate salaries based on features.  
- **Industry Comparison:** Study salary trends across **different sectors** (e.g., Tech vs. Finance).

---

## 🧩 Summary

This project demonstrates a full **data wrangling lifecycle** — from raw data collection to analysis — showcasing how structured techniques can transform unclean, inconsistent data into meaningful business insights. It highlights how **data science roles vary in pay and demand**, providing valuable takeaways for both job seekers and employers in the AI and analytics space.

---
