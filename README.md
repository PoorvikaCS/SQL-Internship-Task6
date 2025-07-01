 Task 6: Subqueries and Nested Queries – SQL Developer Internship

 Objective
To demonstrate mastery of advanced SQL logic using subqueries and nested queries in various clauses including `SELECT`, `WHERE`, and `FROM`.
This task helps build strong foundations for analytical SQL roles.

 Dataset Overview (Employees Table)

| Column      | Type    | Description                    |
| ----------- | ------- | ------------------------------ |
| emp\_id     | INTEGER | Primary Key                    |
| name        | TEXT    | Employee Name                  |
| age         | INTEGER | Employee Age                   |
| department  | TEXT    | HR, IT, Finance, etc.          |
| salary      | INTEGER | Monthly Salary                 |
| bonus       | INTEGER | Performance Bonus              |
| position    | TEXT    | Intern, Analyst, Manager, etc. |
| manager\_id | INTEGER | emp\_id of reporting manager   |

 Key Concepts Applied

* Scalar Subqueries
* Correlated Subqueries
* Subqueries with IN / EXISTS / NOT EXISTS
* Subqueries in SELECT / WHERE / FROM
* Derived Tables

Implemented Queries

| No. | Query Description                                                          |
| --- | -------------------------------------------------------------------------- |
| 1   | Highest salary in each department (Scalar Subquery)                        |
| 2   | Departments with above average salary (Subquery in WHERE)                  |
| 3   | Employees earning more than their manager (Correlated Subquery)            |
| 4   | Employees in top 3 salaries (IN Subquery)                                  |
| 5   | Check if interns exist (EXISTS clause)                                     |
| 6   | Employees who are not managers (NOT EXISTS)                                |
| 7   | Show average company salary beside each employee (SELECT Scalar Subquery)  |
| 8   | Departments with more than 2 employees (Derived Table in FROM)             |
| 9   | Similar names within the same department (Correlated Subquery with EXISTS) |
| 10  | Employees earning above department average (Correlated Subquery in WHERE)  |



💬 Interview Q\&A (Based on Task Guide)

1. What is a subquery?
   A subquery is a query nested inside another SQL query. It helps in filtering, comparing, or calculating values dynamically within the main query.

2. Difference between subquery and join?

* Join combines data from multiple tables based on a condition.
* Subquery runs inside another query and returns results used by the outer query.

3. What is a correlated subquery?
   A subquery that uses a column from the outer query, making it run once for each row in the outer query.

4. Can subqueries return multiple rows?
   Yes. Subqueries using IN, EXISTS, or used in FROM can return multiple rows. Scalar subqueries must return only one.

5. How does EXISTS work?
   EXISTS returns TRUE if the subquery returns any row. It’s often used for checks like "if data exists."

6. How is performance affected by subqueries?
   Correlated subqueries can slow performance as they execute once per outer row. Derived tables and optimized subqueries can help.

7. What is a scalar subquery?
   A subquery that returns exactly one value (one row, one column), often used in SELECT or WHERE.

8. Where can we use subqueries?
   In SELECT, FROM, WHERE, HAVING, and even UPDATE or DELETE clauses.

9. Can a subquery be in FROM clause?
   Yes, and it's known as a derived table or inline view. Useful for grouping and summarization before filtering.

10. What is a derived table?
    A derived table is a subquery used in the FROM clause that acts like a temporary table.

