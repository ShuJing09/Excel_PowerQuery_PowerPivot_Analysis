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

   * _data_jobs_all_ <br>
     <br>
   <img width="298" height="502" alt="image" src="https://github.com/user-attachments/assets/96c6067a-390c-44ec-8f60-5b72e005679e" /> <br>
         <br>
      * _data_jobs_skill_ <br>
        <br>
      <img width="313" height="476" alt="image" src="https://github.com/user-attachments/assets/88f289e5-e03a-4020-85f3-66a425146a08" />

## Load 💻
   * _data_jobs_all_ 
     
   <img width="2549" height="901" alt="image" src="https://github.com/user-attachments/assets/6b5171b8-c2b1-430f-b3e6-e3dfb0d9088c" />

   * _data_jobs_skill_ 
     
   <img width="2550" height="806" alt="image" src="https://github.com/user-attachments/assets/96da1dff-c2a0-4510-a87e-0c46abd12a78" />

## The Analysis 📈
### 1. More Skills = Better Pay?

* 🧮 Added measure useing DAX functions like DIVIDE() for skills per job, MEDIAN() for median salary. <br>

<img width="1116" height="632" alt="image" src="https://github.com/user-attachments/assets/3039dbd1-e828-4ba8-8b9f-def1647ee9c9" /> <br>

1️⃣ The data shows a moderate positive correlation betwween the number of skills and yearly salary among data professionals, especially in technical roles (Data Engineers). \
2️⃣ However, seniority and specialization strongly impact the salary, where the skill count alone doesn’t guarantee higher pay.

## 2. Yearly Salary of Each Jobs in Different Regions


## Pivot Charts




## Power Pivot

## DAX (Data Analysis Expression)


## Conclusion
- 
