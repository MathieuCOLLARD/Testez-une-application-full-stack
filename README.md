# Estate

### Spring Boot configuration : 
- Project Type: Maven
- Java Language Version: 17
- Spring Boot Version: 2.6.1
  
### Dependencies:
- Spring Boot Starter Data JPA
- Spring Boot Starter Security
- Spring Boot Starter Validation
- Spring Boot Starter Web
- MySQL Connector Java (runtime scope)
- JSON Web Token (JJWT)
- Spring Boot Starter Test
- Spring Security Test
- Lombok (optional)

### Build Plugins:
- Spring Boot Maven Plugin
- Jacoco Maven Plugin for code coverage reporting and checking
- Maven Compiler Plugin for configuring Java version compatibility to 9
- Exclusions: Excludes specific packages from code coverage checks in Jacoco

## Start the project

Git clone:

> git clone https://github.com/MathieuCOLLARD/Testez-une-application-full-stack

### Start the front

Open a terminal and check if we are in "Testez-une-application-full-stack/front"

Start the front using this command in a terminal:

> npm run start

### Start the back

Choose com.openclassrooms.api.ApiApplication file in configuration

Start the project using run button in the IDE or using right click on SpringBootSecurityJwtApplication.java file and 'Run SpringBootSecurityJwtApplication.main()'

## Configure the database 

Download mysql with the installer :

> https://dev.mysql.com/downloads/installer/

cd in the mysql folder or use mysql as global variable and run this command :

> 'mysql -u root -p'

Choose the right database using the command

> 'USE _databasename_'

Use the script file in the angular project to create tables and dependencies :

> ressources/sql/script.sql

## Run the tests and generate coverage

### Unitary test (Jest)

Launching test:

> npm run test

for following change:

> npm run test:watch

Generate coverage: 

> npm test -- --coverage

Coverage report avaible here:

> front/coverage/jest/lcov-report/index.html

### Test E2E

Launching e2e test:

> npm run e2e

Generate coverage report (you should launch e2e test before):

> npm run e2e:coverage

Report is available here:

> front/coverage/lcov-report/index.html

### Jacoco Test

Launch and generate the jacoco code coverage :

> mvn clean test

Coverage report available here: 

> back/yoga-app/target/jacoco/index.html

## Ressources

### Postman collection

For Postman import the collection

> ressources/postman/yoga.postman_collection.json 

by following the documentation: 

https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#importing-data-into-postman


### MySQL

SQL script for creating the schema is available `ressources/sql/script.sql`
