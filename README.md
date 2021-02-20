# Pewlett-Hackard-Analysis

## Summary

Created entity relationship diagrams, preformed data modeling, and completed analysis on an emplouee database using SQL. Applied knowledge of DataFrames and tabular data to create an entity relationship diagrams. Then imported data from ERD's into postgres database. Lastly, created quires that use data to anser questions for Pewlett Hackerard managment. 

## Overview of the analysis 

### The Number of Retiring Employees by Title 

- Used the ERD and SQL queries to create a Retirement Titles table that holds all the titles of current employees who were born between January 1, 1952 and December 31, 1955. Because some employees may have multiple titles in the database—for example, due to promotions, used the DISTINCT ON statement to create a table that contains the most recent title of each employee. Then, used the COUNT() function to create a final table that has the number of retirement-age employees by most recent job title.

### The Employeese Eligible for the Menetorship Program 

- Used the ERD and SQL queries, created a mentorship-eligibility table that holds the current employees who were born between January 1, 1965 and December 31, 1965.

## Results 

![retirement_titles](https://user-images.githubusercontent.com/16258584/99162094-40a38780-26bf-11eb-9274-8b65260be1cc.png)

- Created the retirment titles page to get the list of people who could be possibly retiring based of off the year that they were born. The error in this table was that it did not get rid of duplicate names so the final number count would have been inaccurate using this table 

![unique_titles](https://user-images.githubusercontent.com/16258584/99162074-ed313980-26be-11eb-903a-f8cc644603a6.png)
 
- This lead me to creating the unique titles table. This is the accurate number of people who could retire based on their age and ordered by their employee numbers. 

![retiring_titiles](https://user-images.githubusercontent.com/16258584/99162088-2c5f8a80-26bf-11eb-9474-131c8535456a.png)

- The retiring titles uses the counts the different titles in the unique titles tab for the analysis.

![mentorship_eligibility](https://user-images.githubusercontent.com/16258584/99162099-5749de80-26bf-11eb-8fae-f8d80191a471.png)

- The mentorship eligibility table list the employees who are eligible to participate in a mentorship program by employee number.

![mentorship_count](https://user-images.githubusercontent.com/16258584/99162444-7ba7ba00-26c3-11eb-9641-2c5fc444b887.png)

- The mentorship count of employees by title. 

## Summary 
- How many roles will need to be filled as the "silver tsunami" begins to make an impact?

![retiring_titiles](https://user-images.githubusercontent.com/16258584/99162088-2c5f8a80-26bf-11eb-9474-131c8535456a.png)

- Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

- There are currently not enough employees in the departments shown by the mentorship count.
