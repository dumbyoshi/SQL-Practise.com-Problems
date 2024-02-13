# SQL-Practise.com-Problems
Here i have uploaded the sql problems and its solution from a website sql-practise.com ,solved on daily basis.






Problem 1 :
Show first name, last name, and gender of patients whose gender is 'M' 
Solution :
~~~~sql
SELECT first_name,
       last_name,
       gender
FROM patients
WHERE gender = 'M';
~~~~
-------------------------------------------------------------------------------------------------
Problem 2 
Show first name and last name of patients who does not have allergies. (null)
Solution :
~~~~sql
SELECT first_name,lastname
     FROM patients 
WHERE allergies IS null;
~~~~
-------------------------------------------------------------------------------------------------
Problem 3
Show first name of patients that start with the letter 'C'
Solution:
~~~~sql
SELECT first_name
FROM patients
WHERE first_name LIKE 'C%';
~~~~
Another Solution:
~~~~sql
SELECT first_name
FROM patients
WHERE substring(first_name, 1, 1) = 'C'
~~~~
------------------------------------------------------------------------------------------------
Problem 4
Show first name and last name of patients that weight within the range of 100 to 120 (inclusive)
Solution:
```sql
select first_name , last_name 
from patients
where weight <= 120 
AND weight  >= 100;
```
-------------------------------------------------------------------------------------------------

Problem 5 
Update the patients table for the allergies column. If the patient's allergies is null then replace it with 'NKA'
Solution:
```sql
UPDATE patients 
set allergies = 'NKA'
where allergies is null;
```
-------------------------------------------------------------------------------------------------










