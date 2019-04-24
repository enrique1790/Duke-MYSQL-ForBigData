Managing Big Data With MYSQL: Outline
Week 1: Entity-Relationship Diagrams & Relational Schema 
Week 2: SQL Syntax - Select, where, from, order by, limit, operations
Week 3: OPERATORS: SUM, AVG, DISTINCT, COUNT
*Restrictions: HAVING, GROUP BY
* Inner Joins & Outer Joins:
Week 4 - Subqueries & Operators - Not, And, OR,IF, CASE
Week 5: Final Week - Dillard's Database Exercises

Typical Syntax Follows this order
SELECT item
FROM table
WHERE condition
GROUP BY variable
HAVING condition
ORDER BY category ASC / DESC

Week 2: Commands
[Statement]
Select:The data I want
From: These database and tables

Where: WHERE- is used with SELECT statement to extract only those records that fulfill specified conditions.
Group (By) - The GROUP BY statement is often used with aggregate functions (COUNT, MAX, MIN, SUM, AVG) to group the result-set by one or more columns.
Having: The HAVING clause was added to SQL because the WHERE keyword could not be used with aggregate functions.
Order (BY) - This field or list; in [ASC | DESC] order.
Distinct:  eliminate all the duplicate records and fetching only unique records.
AS: The AS clause allows you to assign an alias (a temporary name) to a table or a column in a table.
IS Not Null: query to only select rows that do not have null values
Upper: all of the distinct breed names in UPPER case
Operations : Arithmetic | Comparison | Logical | Operators used to negate conditions

Week 3 Commands
[Operators, Aggragate]
SUM:  function returns the total sum of a numeric column.
AVG: function returns the average value of a numeric column.
DISTINCT: is used to return only distinct (different) values. Inside a table, a column often contains many duplicate values; and sometimes you only want to list the different (distinct) values.
COUNT: function returns the number of rows that matches a specified criteria.

[Restrictions]
HAVING: The HAVING clause was added to SQL because the WHERE keyword could not be used with aggregate functions
GROUP BY: statement is often used with aggregate functions (COUNT, MAX, MIN, SUM, AVG) to group the result-set by one or more columns.

[Joins]
Inner Joins: keyword selects records that have matching values in both tables.
Outer Joins: keyword return all records when there is a match in either left (table1) or right (table2) table records.
Note: FULL OUTER JOIN can potentially return very large result-sets!
Tip: FULL OUTER JOIN and FULL JOIN are the same.

Week 4 - Commands
[Subqueries]
Subqueries, which are also sometimes called inner queries or nested queries, are queries that are embedded within the context of another query. They are useful for complex queries, and also for testing smaller parts of the queries to ensure they give you what you want first before assembling the whole thing.

Some basic rules are:
*ORDER BY phrases cannot be used in subqueries (although ORDER BY phrases can still be used in outer queries that contain subqueries)

*Subqueries in SELECT or WHERE statements can output no more than 1 row. Otherwise, subqueries in SELECT or WHERE clauses that return more than one row must be used in combination with operators that are explicitly designed to handle multiple values, such as the IN operator.

*Lastly, when they are used in FROM clauses, they create what are called derived tables. This comes into play later when you want to optimse your query to run faster. Having smaller derived tables helps the query be answered quicker because the db does not need to hold such a large derived table in memory. But for now, focus on writing the damn thing right first.

[Operators]
NOT - The NOT operator reverses the meaning of the logical operator with which it is used. Eg: NOT EXISTS, NOT BETWEEN, NOT IN, etc. This is a negate operator
AND - The AND operator is a logical operator that combines two conditions and returns TRUE only if both condition evaluate to TRUE . The AND operator is often used in the WHERE clause of the SELECT, UPDATE, DELETE statement to form conditions to filter the result set.
OR - a logical operator that combines two conditions, but it returns TRUEwhen either of the conditions is TRUE.
Note: You can also combine AND and OR to create complex conditional expressions.
IF - The IF() function returns a value if a condition is TRUE, or another value if a condition is FALSE. 

CASE: The CASE statement goes through conditions and return a value when the first condition is met (like an IF-THEN-ELSE statement). So, once a condition is true, it will stop reading and return the result.
*If no conditions are true, it will return the value in the ELSE clause.
*If there is no ELSE part and no conditions are true, it returns NULL.

Week 5: Final Week - Dillard's Database Exercises
