exercise 1 - Select all records from the Students table where the second letter of the City is an "a".
select * from Students Where City Like '_a%';

exercise 2 - Select all records from the Students table where the first letter of the City is an "a" or a "c" or an "s".
select * from Students Where City Like 'a%' or City Like 'c%' or City Like 's%';

exercise 3 - Select all from the Students table records where the first letter of the City starts with anything from an "a" to an "f".
select * from Students Where City Like 'a%' or City Like 'b%' or City Like 'c%' or City Like 'e%' or City Like 'f%';

exercise 4 - Select all records from the Students table where the first letter of the City is NOT an "a" or a "c" or an "f".
select * from Students Where City Not Like 'a%' and City Not Like 'c%' and City Not Like 's%' and City Not Like 'f%';

exercise 5 - Use the IN operator to select all the records from the Students table where Country is either "Sint Maarten" or "Haiti".
select * from Students Where Country In ('Sint Marteen', 'Haiti');

exercise 6 - Use the IN operator to select all the records from the Students table where Country is NOT "Sint Maarten" and NOT "Haiti".
select * from Students Where Country Not In ('Sint Marteen', 'Haiti');

exercise 7 - Use the BETWEEN operator to select all the records from the Courses table where the value of the CreditHours column is between 10 and 20.
select * from Students Where CreditHours Between 10 and 20;

execrise 8 - Use the BETWEEN operator to select all the records from the Courses table where the value of the CreditHours column is NOT between 10 and 20.
select * from Students Where CreditHours Not Between 10 and 20;

exercise 9 - Use the BETWEEN operator to select all the records from the Courses table where the value of the CourseName column is alphabetically between 'ColdFusion' and 'Python'.
select * from Students Where CourseName Between 'ColdFusion' and 'Python';

exercise 10 - When displaying the Students table, make an alias of the PostalCode column, the column should be called Zip instead
Select PortalCode AS Zip from table Students;

exercise 11 - When displaying the Students table, refer to the table as Learners instead of Students.


Select 'PortalCode' AS 'Zip' from table Students as 'Learners';
