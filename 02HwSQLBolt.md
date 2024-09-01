# <span style='color:cyan' >SQLBolt Homework</span>
### <span style='color:magenta' >SQL Review: Simple SELECT Queries</span> 

#### 1. Find the longest time that an employee has been at the studio.

`SELECT` 
    
   `MAX`(years_employed) as longest_employment_time 
    
`FROM` employees;

#### 2. For each role, find the average number of years employed by employees in that role.

`SELECT` 
    
   role, `AVG`(years_employed) as avg_employment_years_per_role

`FROM` employees

`GROUP BY` role;

#### 3.Find the total number of employee years worked in each building.

`SELECT`
    building, `SUM`(years_employed) AS total_years_employed

`FROM` employees

`GROUP BY` building;
