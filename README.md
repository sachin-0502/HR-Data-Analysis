# HR-Data-Analysis
[LINK TO THE INTERACTIVE DASHBOARD](https://public.tableau.com/views/HRAnalyticsDashboardTableau_17088590617720/Dashboard1?:language=en-US&publish=yes&:sid=&:display_count=n&:origin=viz_share_link)

### Snap of the dashboard <p> </p>

![image](https://github.com/sachin-0502/HR-Data-Analysis/assets/144464445/95e3df2c-14b6-486f-9f35-360ec5b12372)

### Project Outcome
The dashboard was created using a available public dataset of HR department and generated meaningful insights by considering the sample data as a orginal data from an organization. Thus learned about various terms and features related to HR department including attrition variables, number of job satisfaction features and other.

### The dashboard is created using BI tool - TABLEAU.

## About dataset
This is a sample public dataset which consists 1470 rows and 39 columns in a csv file describing about how an organization's HR department handles its data for all the employees working or worked here. Some important columns are described below:

- Attrition =  the column "Attrition" with values "Yes" or "No" likely indicates whether an employee has left the company ("Yes") or is still employed with the company ("No").
- CF_Age_Band = the employee refers to which age band (25-34, 35-44, 45-54, over 55, under 25)
- Department = Sales/ R&D/ HR ( employee working in department)
- Education field = employee got the education in which field ( Human Resources/ Life Science/ Marketing/ Medical/ Technical Degree/ Other )
- Gender = Male/ Female
- Job Role = Healthcare Representative/ Human Resources/ Lab Technician/ Manager/ Manufacturing Director/ Research Director/ Research Scientist/ Sales Executive/ Sales Representative
- Mairtal Status = Married/ Single
- Age = Actual Age of employee
- Job Satisfaction = 0 to 5
- etc.

 # Steps followed for making main dashboard
 1. Load data into Tableau
 2. Changed datatype of some columns
 3. Measures Calculation
 - Tableau automatically detects and provide the useful measures but that are not quite appropriate sometimes as per our requirment. Thus I created some measures manually in order to achieve the desired insights.
 - Attrition Count = IF([Attrition])='Yes' THEN 1 ELSE 0 END
 - Active Employees = SUM([Employee Count]) - SUM([Attrition Count])
 - Attrition Rate = SUM([Attrition Count]) / SUM([Employee Count])
 - Average Age = SUM([Age]) / SUM([Employee Count])
   
 4. Created 7 worksheets for different visuals describing insights in a detailed view
    - KPI ( Employee Count, Attrition Count, Attrition Rate, Active Employees, Average Age, Average Daily Rate ) <p> </p>
    - ![image](https://github.com/sachin-0502/HR-Data-Analysis/assets/144464445/4363555d-8405-4d34-b0b0-682760ee81b2)

    - Horizontal Column Chart ( Attrition By Gender ) <p> </p> ![image](https://github.com/sachin-0502/HR-Data-Analysis/assets/144464445/7ddf604c-8876-4bd2-adbc-6974d9c832e7)

    - Pie Chart ( Department wise attrition ) <p> </p> ![image](https://github.com/sachin-0502/HR-Data-Analysis/assets/144464445/b550188c-7c26-4dcd-b7f3-c79c291a8daf)

    - Bar chart ( no. of employees by age group ) Created Age bin by ( go to the age column and right click --> create --> bins --> select bin size ) <p> </p>
    ![image](https://github.com/sachin-0502/HR-Data-Analysis/assets/144464445/820ca978-a101-4fbe-832d-d34dc97d415c)

    - Heat map (Job Satisfaction rating with number of employees based on job role) <p> </p> ![image](https://github.com/sachin-0502/HR-Data-Analysis/assets/144464445/a1e5e582-b9b3-409f-a7a0-24480c80b952)

    - Column horizontal Chart ( Education field wise attrition ) <p> </p> ![image](https://github.com/sachin-0502/HR-Data-Analysis/assets/144464445/82e690e0-5604-493e-ad09-abf80a4d0871)

    - Pie charts ( Attrition number by age band ) <p> </p> ![image](https://github.com/sachin-0502/HR-Data-Analysis/assets/144464445/b36342f5-02a1-4875-af71-4bc01c8042e9)
   
  5. Load the dashboard background in the dashboard canvas area.
  6. Make dashboard by activate floating option in the dashboard canvas so that every chart can be drag anywhere.
  7. Then drag all the created worksheet visuals in the dashboard canvas by doing necessary formatting.
  8. Place the visuals in right manner at right place.
  9. Add interactive filter of the field "department" which will work as a slicer in the dashboard and in all the visuals the action filters will be auto working in the dashboard.
  10. Publish the report on tableau public. 

   
