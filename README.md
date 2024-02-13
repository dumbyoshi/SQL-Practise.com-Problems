# SQL-Practise.com-Problems
Here i have uploaded the sql problems and its solution from a website sql-practise.com ,solved on daily basis.






Problem 1 :
Show first name, last name, and gender of patients whose gender is 'M' 
Solution :
```sql
SELECT first_name,
       last_name,
       gender
FROM patients
WHERE gender = 'M';
```
-------------------------------------------------------------------------------------------------
Problem 2 
Show first name and last name of patients who does not have allergies. (null)
Solution :
'''sql
SELECT first_name,lastname
FROM patients 
WHERE allergies IS null;
'''
-------------------------------------------------------------------------------------------------
Problem 3
Show first name of patients that start with the letter 'C'
Solution:
'''sql
SELECT first_name
FROM patients
WHERE first_name LIKE 'C%';
'''
------------------------------------------------------------------------------------------------
