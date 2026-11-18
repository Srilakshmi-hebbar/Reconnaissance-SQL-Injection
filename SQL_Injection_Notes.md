
# SQL Injection Notes

## 1. What is SQL Injection?
SQL Injection (SQLi) is a web application vulnerability that occurs when user input is incorrectly included in database queries. An attacker may manipulate the query and affect how the application interacts with its database.

## 2. How It Happens
SQL injection can occur when an application directly combines user input with SQL statements instead of handling the input safely.

## 3. Lab Observation
During testing in the local bWAPP environment, an apostrophe was entered into the SQL injection testing field.

The application displayed a database-related error message.

This observation suggests that the input affected database query processing. However, an error message alone does not prove that SQL injection is exploitable.

## 4. Possible Impact
If a SQL injection vulnerability is confirmed, it may lead to:
- Unauthorized access to database information.
- Modification or deletion of records.
- Authentication bypass.
- Exposure of sensitive information.

## 5. Prevention Techniques
- Use parameterized queries and prepared statements.
- Validate user input.
- Apply least-privilege permissions to database accounts.
- Avoid displaying detailed database errors to users.
- Perform regular security testing.

## 6. Conclusion
This exercise provided an introduction to SQL injection and demonstrated why secure input handling is important in web applications.
