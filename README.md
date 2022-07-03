# example-mule-project
A Mule flow that queries database upon receiving http request and returns resultset in csv format

# Prerequisites
1. Google search and download Mule Anypoint Studio. It's nothing but Eclipse editor with special features and support for Mule project development.
2. Create a database in Oracle with a table as per below structure.
```
CREATE TABLE Person (
    PersonID int,
    LastName varchar(255),
    FirstName varchar(255)
);
```

# Setup and execution
1. Checkout and import this project into your "Mule Anypoint Studio" IDE.
2. Build it just as you would build any other Eclipse project.
3. Right click on `example-mule-project.xml` and select Run As > Mule Application
4. Open eb browser and hit URL http://localhost:8080/oracle.csv
