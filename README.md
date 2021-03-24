# [Deskera](https://www.deskera.com) Coding Test

## Problem Statement
Implement an Employee Manager for a Company so that the HR Admins can
1. Add a new Employee
2. Find any Employee by Employee Id
3. Find all Employees older than X years (So if X = 30 then all employee who are older than 30 years. For e.g. Employees with age 31, 32, 40, etc but employees with age 30 years are not included)
3. Delete any Employee at the time of employee exit
4. List all the current Employees

### Things to remember
1. When an Employee is added, the information being provided is `Full Name` and `Birth Date`. These are mandatory fields.
2. The system must store `First Name` and `Last Name` separately in the `Employee` object
3. The system must store `ageInYears` and `ageInMonths` separately in the `Employee` object
3. `Full Name` can have names such `John`, `John Doe`, `John P. Doe`, `John Paul Doe`. The way to break the names down in first name and last name are as follows
   | Full Name     | First Name    | Last Name  |
   | ------------- |---------------| ------------|
   | John     | John |  |
   |John Doe      | John      |   Doe |
   | John P. Doe | John P.     |    Doe |
   | John Paul Doe | John Paul     |    Doe |
4. No two employees with same `Full Name` and `Birth Date` are allowed i.e. We can not have 2 `John Doe` born on `1-Jan-1990`
5. `Employee Id` has to be generated by the system and for every new employee a new and unique employee id must be generated
6. Accetable format for `Birth Date` is `DD-MON-YYYY`. For e.g. `1-Jan-1990`, `2-Feb-1991`. Other formats such as `Jan-1-1990`, `01-01-1990`, `1990-01-01`, must not be accepted by the system
7. `ageInYears` and `ageInMonths` should be rounded up. For e.g. a person born on `1-Jan-2020` will have `ageInYears` as `2` and `ageInMonths` as `15`

## Instructions
1. The EmployeeManager is in [src/EmployeesManager.java](./src/EmployeesManager.java)
2. The implement must be in this file only and no new files can be added to the code
3. Only Java SDK can be used and no other dependencies/ library can be used
4. `Fork` the repository, keep it public and while submission, provide your repository URL.
