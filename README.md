# Excel_PowerQuery_PowerPivot_Analysis

# Tools Used 🔧

⚙️ Power Query \
🧩 Power Pivot \
📊 Pivot Tables and Pivot Charts \
🧮 DAX (Data Analysis Expressions)

# Project : Questions to Answer ❓
1. Do more skills get you better pay?
2. What’s the salary for data jobs in different regions?
3. What are the top skills of data professionals?
4. What’s the pay for the top 10 skills?

   
# ⚙️ Power Query : Extract, Transform and Load Data
## Extract 📥
- Extract the data from Excel Workbook (_data_salary_all.xlsx_) and create two queries: \
   * First query, _data_jobs_all_ that contains all job information.
   * Second query, _data_jobs_skills_ that consists the skills for each job ID.

## Transform 🔄
- Transform the data by changing column type, trimming text, inserting custom & conditional columns, spliting text by delimeter and unpivoting columns. 

   * ```data_jobs_all``` <br>
     <br>
   <img width="298" height="502" alt="image" src="https://github.com/user-attachments/assets/96c6067a-390c-44ec-8f60-5b72e005679e" /> <br>
         <br>
   * ```data_jobs_skill```  <br>
     <br>
      <img width="313" height="476" alt="image" src="https://github.com/user-attachments/assets/88f289e5-e03a-4020-85f3-66a425146a08" />

## Load 💻
   * ```data_jobs_all``` 
     
   <img width="2549" height="901" alt="image" src="https://github.com/user-attachments/assets/6b5171b8-c2b1-430f-b3e6-e3dfb0d9088c" />

   * ```data_jobs_skill``` 
     
   <img width="2550" height="806" alt="image" src="https://github.com/user-attachments/assets/96da1dff-c2a0-4510-a87e-0c46abd12a78" />

## The Analysis 📈
### 1. More Skills = Better Pay?

* 🧮 Created measures using DAX functions like DIVIDE() for skills per job, MEDIAN() for median salary. <br>

<img width="1116" height="632" alt="image" src="https://github.com/user-attachments/assets/3039dbd1-e828-4ba8-8b9f-def1647ee9c9" /> <br>

1️⃣ The data shows a moderate positive correlation betwween the number of skills and yearly salary among data professionals, especially in technical roles (Data Engineers). 
<br>
2️⃣ However, seniority and specialization strongly impact the salary, where the skill count alone doesn’t guarantee higher pay.

## 2. Yearly Salary of Each Jobs in Different Countries

* 🧮 Created measures using DAX functions CALCULATE() for median salary in the United States, and slicer to filter different countries <br>
 
 ```
=CALCULATE(
    MEDIAN(data_jobs_all[salary_year_avg]),
    data_jobs_all[job_country] = "United States")
```
<br>
<img width="2011" height="790" alt="image" src="https://github.com/user-attachments/assets/2be82502-1ff8-43d8-86e3-08e29897c0b1" /> <br>

<br>

1️⃣ US salaries are consistently the highest across all roles, showing that US has a very mature tech market with higher competition for talent, massive companies budgets and higher venture capital.
<br>
2️⃣ Singapore's salary varies strongly by job type. For instance, Data Scientist and Senior Data Scientist pays are slightly higher than US and Non-US, likely due to high demand in finance & trading firms and shortage of talent.
<br>
3️⃣ Comparing Singapore to US job salaries, there's a huge gap of salaries in roles: 
   * Software Engineer (May due to Silicon Valley and FAANG sets high salary floor, and Singapore has far fewer tech companies compared to the US)
   * Machine Learning Engineer (May due to premium pay in the US as AI development is booming)
   * Cloud Engineer (May due to DevOps & Cloud migration boom in the US that leads to higher pay. ❗HOWEVER, Singapore's salary data needs further investigation as the engineers' pay is lower than analyst)<br>

4️⃣ The pays are competitive when it comes to seniority roles in all regions, indicating senior tech talent is highly valued everywhere.


## Top Skills for Data Professionals

🧩 Used Power Pivot to create relationship between 2 queries ```data_jobs_all``` & ```data_jobs_skill``` on ```job_id``` (created indexes in ⚙️ Power Query ETL process) <br>

<img width="1090" height="950" alt="image" src="https://github.com/user-attachments/assets/73977db0-b41b-40ca-803e-4bf47f5c19af" /> <br>

📊 Insert Pivot Tables and Pivot Chart by loading data from Data Model. <br>

<img width="848" height="518" alt="image" src="https://github.com/user-attachments/assets/d01c8145-ff68-46a2-aa08-8e2c792dc957" /> <br>

1️⃣ SQL and Python dominate as top skills in data-related jobs, reflecting its foundational importance to most job opportunities.
<br>
2️⃣ The prominence of AWS and Azure in job postings highlights how organizations are rapidly moving toward cloud infrastructure and big data ecosystems.
<br>
3️⃣ Utilization of Spark and Snowflake to build powerful and scalable data pipelines, indicates the essentiality to process big data for effecient data analytics.


## Pay for Top Skills




## Conclusion
- 
