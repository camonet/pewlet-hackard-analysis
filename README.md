# pewlett-hackard-analysis


<!-- 14 to >12.0 pts
Demonstrating Proficiency
✓The purpose is well defined. 
✓There is a bulleted list that addresses FOUR major results. 
✓The summary addresses the TWO questions and contains TWO additional queries or tables. -->
## Purpose
The purpose of this analysis was to use SQL, PostgreSQL and pgAdmin to aid in creating new files based off existing data. This new assignment consists of two technical analysis deliverables and a written report
- Deliverable 1: The Number of Retiring Employees by Title
- Deliverable 2: The Employees Eligible for the Mentorship Program
- Deliverable 3: A written report on the employee database analysis (README.md)

## Results
### Retiring Titles 
- <img width="213" alt="image" src="https://user-images.githubusercontent.com/99444856/175793901-5f4cf60c-0dbd-4ec3-a76b-1469c303f4c5.png">
The number of retiring employees from each department is shown above. (72,458 employees)
- <img width="213" alt="Screen Shot 2022-06-25 at 6 56 06 PM" src="https://user-images.githubusercontent.com/99444856/175794007-854131c3-0eec-4c27-9eaa-922100581f20.png">
The number of current employees is shown above. (579,308 total employees) 
- The number of employees eligible for retirement accounts for 12.5% of the pewlett-hackard workforce
- The number of mentorship eligible employees is 1510

## Summary 
How many roles will need to be filled as the "silver tsunami" begins to make an impact?
- 72,458 employee roles will need to be filled as the silver tsunami begins to make an impact. I found this out by finding the number of total employees using the query: 

current emp:

SELECT COUNT (ti.title), 
ti.title
INTO titles1
FROM titles as ti
GROUP BY ti.title
ORDER BY COUNT DESC;

SELECT * FROM titles1

to get the following table:
<img width="213" alt="Screen Shot 2022-06-25 at 7 14 38 PM" src="https://user-images.githubusercontent.com/99444856/175794356-b8fe9dcd-2b04-47ac-a8d0-b73ee943a4e6.png">

Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

Because there are only 1510 employees eligible for mentorship, at the moment, there will not be enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees. 

