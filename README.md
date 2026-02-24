
# 📊 Excel Data Jobs Dashboard

*final dashboard preview:*
<img width="1855" height="821" alt="final-data-job-dashboard" src="https://github.com/user-attachments/assets/ffccfee2-46c0-4939-a00e-5d33a878e9e6" />

## Introduction
This data jobs salary dashboard was created to help job seekers investigate salaries for their desired jobs and ensure they are being adequately compensated. 
The data is from my Excel course, which provides a foundation in analyzing data using this powerful tool. The data contains detailed information on job titles, salaries, locations, and essential skills that are presented here.

### Dashboard File
My final dashboard is available here:  
👉 [View Dashboard](./microsoft-excel-files)

### Data Jobs Dataset

The dataset used for this project contains 30.000+ rows real-world data science job information from 2023. It includes detailed information on job titles, salaries, locations, and skills.  
👉 [View Dataset](./datasets)

## 🎯 Key Objectives  

- Analyse salary trends across data roles  
- Build an interactive dashboard  
- Apply formulas for dynamic insights  
- Present findings through visualisations  

### 🛠️ Skills Demonstrated  

- Data visualisation (charts & dashboard design)  
- Advanced Excel formulas and functions 
- Data validation & interactivity  
- Data cleaning and preparation  
- Analytical thinking  

## 📊 Dashboard Highlights  

- Interactive filters for job title, country, and schedule type  
- Salary comparison across roles  
- Geographic salary distribution  
- Dynamic calculations based on user input  

## 🔍 Key Insights  

- Senior and engineering roles show higher median salaries  
- Salaries vary significantly by country  
- Job schedule type influences compensation  

## 🧠 What This Project Shows  

This project highlights my ability to:  

- Turn raw data into meaningful insights  
- Build clean and user-friendly dashboards  
- Communicate findings through visual storytelling  
- Use Excel as a data analysis tool  

## 📌 Tools  

- Microsoft Excel 

## Dashboard Build

### 📉 Charts

#### 📊 Data Jobs Salaries - Bar Chart

<img width="433" height="250" alt="salary-bar-chart" src="https://github.com/user-attachments/assets/d8448f82-2ebc-4727-8e97-1b3befa68cc3" />

- 🛠️ **Excel Features:** Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
- 🎨 **Design Choice:** Horizontal bar chart for visual comparison of median salaries.
- 📉 **Data Organization:** Sorted job titles by descending salary for improved readability.
- 💡 **Insights Gained:** This enables quick identification of salary trends, noting that Senior roles and Engineers are higher-paying than Analyst roles.

#### 🗺️ Country Median Salaries - Map Chart

<img width="421" height="250" alt="map-chart" src="https://github.com/user-attachments/assets/99b778cd-8912-4d73-bc7a-e2ea82c62c97" />

- 🛠️ **Excel Features:** Utilized Excel's map chart feature to plot median salaries globally.
- 🎨 **Design Choice:** Color-coded map to visually differentiate salary levels across regions.
- 📊 **Data Representation:** Plotted median salary for each country with available data.
- 👁️ **Visual Enhancement:** Improved readability and immediate understanding of geographic salary trends.
- 💡 **Insights Gained:** Enables quick grasp of global salary disparities and highlights high/low salary regions.

#### 📊 Job Schedule Type - Bar Chart
<img width="371" height="250" alt="job-schedule-type-bar-chart" src="https://github.com/user-attachments/assets/e15b67fa-d926-4967-a628-0c045ab4e344" />

- 🛠️ **Excel Features:** Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
- 🎨 **Design Choice:** Horizontal bar chart for visual comparison of median salaries.
- 📉 **Data Organization:** Sorted job titles by descending salary for improved readability.
- 💡 **Insights Gained:** This enables quick identification of salary trends, noting that full-time are higher-paying than other job schedule types.


### 🧮 Formulas and Functions

#### 💰 Median Salary by Job Titles

```
=MEDIAN(
IF(
    (jobs[job_title_short]=A2)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type])))*
    (jobs[salary_year_avg]<>0),
    jobs[salary_year_avg]
)
)
```

- 🔍 **Multi-Criteria Filtering:** Checks job title, country, schedule type, and excludes blank salaries.
- 📊 **Array Formula:** Utilizes `MEDIAN()` function with nested `IF()` statement to analyze an array.
- 🎯 **Tailored Insights:** Provides specific salary information for job titles, regions, and schedule types.
- **🔢 Formula Purpose:** This formula populates the table below, returning the median salary based on job title, country, and type specified.


#### ⏰ Count of Job Schedule Type

```
=FILTER(J2#,(NOT(ISNUMBER(SEARCH("and",J2#))+ISNUMBER(SEARCH(",",J2#))))*(J2#<>0))
```

- 🔍 **Unique List Generation:** This Excel formula below employs the `FILTER()` function to exclude entries containing "and" or commas, and omit zero values.
- **🔢 Formula Purpose:** This formula populates the table below, which gives us a list of unique job schedule types.



### ❎ Data Validation

#### 🔍 Filtered List

- 🔒 **Enhanced Data Validation:** Implementing the filtered list as a data validation rule under the `Job Title`, `Country`, and `Type` option in the Data tab ensures:  
      🎯 User input is restricted to predefined, validated schedule types  
      🚫 Incorrect or inconsistent entries are prevented  
      👥 Overall usability of the dashboard is enhanced  


    - job title filter:

        <img width="330" height="276" alt="job-title-filter" src="https://github.com/user-attachments/assets/c4e9516f-62c4-4f54-9ef6-51ed56f9978a" />



    - country filter:

        <img width="281" height="301" alt="country-filter" src="https://github.com/user-attachments/assets/c42946fa-c6a8-4d94-aad3-51601d19e419" />



    - job type filter:

        <img width="327" height="183" alt="type-filter" src="https://github.com/user-attachments/assets/b12c7b0a-3849-45c3-8dbb-2ccccc50e4a2" />  



## Conclusion

I created this dashboard to showcase insights into salary trends across various data-related job titles. This dashboard allows users to make informed decisions about their career paths. Exploring the functionalities to understand how location and job type influence salaries. 


---
## 🌟 About Me

Hi there! I'm **Novia Noer Ramdiany**. I’m passionate on data fields.

Let's stay in touch! Feel free to connect with me on LinkedIn: https://www.linkedin.com/in/noviaramdiany/

