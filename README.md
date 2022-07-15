# JDBC: Project setup

### Description

Create a JDBC automation project

#### Theory:

* Java DataBase Connectivity (JDBC)
* JDBC drivers
* Factory and Singleton design patterns
* Java try with resources
 

#### Practical tasks:
**Task 1**
Description: Create an automation project using Java 11 and Maven. Find and add the appropriate JDBC driver that:
* is compatible with the target DB
* is compatible with Java 11

All connection properties (URL, user, password, etc) should be retrieved from a config properties file.

**Task 2** Description: Factory Helper: Create a database connection that is then automatically closed in a try-with-resources statement

**Task 3** Description: Singleton Helper: Create a database connection before tests start and close it after the last test is executed
Description: Using the Singleton Desing Pattern, create a database helper class with a method that makes and returns a single database connection. A new connection is created only if the old one gets closed and is not alive anymore. Connection is created before all tests and closed at the end of the test execution.
Description: Using Factory Design Pattern, create a database helper class with a createConnection() method that returns a new database connection. We will make a new connection to the DB each time we need it. This connection can then be automatically closed by a try-with-resources statement (database connections have the AutoCloseable interface pre-implemented).
### Instruction
#### Prerequisites
1. SQL: Local database environment setup.
2. customers table with example data
##### Useful links:
https://www.tutorialspoint.com/design_pattern/factory_pattern.htm
https://www.tutorialspoint.com/design_pattern/singleton_pattern.htm
https://www.tutorialspoint.com/jdbc/index.htm