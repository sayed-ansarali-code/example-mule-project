# example-mule-project
A Mule flow that queries database upon receiving http request and returns resultset in csv format

# Prerequisites
1. Google search and download Mule Anypoint Studio. It's nothing but Eclipse editor with special features and support for Mule project development.
2. Create a database in Oracle with a table as per below structure.
```
CREATE TABLE Person (
    PersonID int,
    FirstName varchar(255),
    LastName varchar(255)
);
insert into person values (1, 'firstname1', 'lastname1');
insert into person values (2, 'firstname2', 'lastname2');
insert into person values (3, 'firstname3', 'lastname3');
commit;
```

# Setup and execution
1. Checkout and import this project into your "Mule Anypoint Studio" IDE.
2. Build it just as you would build any other Eclipse project.
3. Right click on `example-mule-project.xml` and select Run As > Mule Application
4. Open web browser and hit URL http://localhost:8080/oracle.csv
5. oracle.csv file containing data from person table should download
