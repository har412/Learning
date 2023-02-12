# SQL Agregate functions

- SQL Aggregate Functions: SUM(), COUNT(), AVG()

- What Is an Aggregate Function in SQL?

- An aggregate function in SQL performs a calculation on multiple values and returns a single value. SQL provides many aggregate functions that include avg, count, sum, min, max, etc. An aggregate function ignores NULL values when it performs the calculation, except for the count function. 
## Max,Min , Avg , Count, Sum ,Group by , where clause, As , DROP , TRUNCATE 
- TRUNCATE TABLE statement is used to remove all rows from a table, effectively emptying it. The TRUNCATE TABLE statement is similar to the DELETE statement, but it is generally faster and more efficient, especially for large tables, because it doesn't log each individual row deletion.
``` 
TRUNCATE TABLE table_name; 
```
Here is the basic syntax for the TRUNCATE TABLE statement:
![](./images/table.png)

- find max salary in employee table?
- ` Select max(salary) from employee`
- find no of rows in table?
- `select Count(*) from employee`
- find total no of departments in oeganization(DISTINCT)?
- `select distinct(Dept) from employee`
- Find SUM salary given by employer
- `select sum(salary) from employee`
- Find AVERAGE Salary given by company ?
- `Select Avg(Salary) from employee `
- GROUP BY Find no of employee in each dept?
- `select dept , count (dept) from emp GROUP BY Dept `
- find all dept whose employee count is less than 2 ?
- `select dept from emp GROUP BY dept
HAVING count(*)<2`
- find name of that person aslo who works in dept where count of employee < 2?
- `Select E_name from Emp where dept in 
(Select dept from Emp group by dept having count(*)<2)`

# Second Table
![](./images/university%20student.png)
- Find max stipend offered by university?
- Find no of students in table?
- find no of subject in university?
- find total stipend given by university?
- Find Averyage stipend offered by the university?
- Find no of students studying each subject?

