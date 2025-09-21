# 2nd_SEM_FINALE_PROJECT



### 1. Project Description
### Purpose of the Project

This is a  system for managing agricultural and animal operations.
From the structure and files, it’s designed as a Farm System with JWT-based security.

### Key Features (based on controllers & entities)

### Authentication & Security

* AuthUserController, JWTConfigFilter, SequrityConfig

* Implements JWT login/authentication to secure APIs.

* Manages user roles (e.g., administrative, manager, scientist, staff).

### User & Staff Management

UserController, StaffController

Create, update, delete, and manage users and staff.

Staff roles (StaffRole.java) define different permissions/responsibilities.

### Field,planand animal Management

FieldController, AnimalController

Manage fields, assign animals and plants to fields.

Handle plants and animal data (planting, harvesting, etc.).

### Equipment & Vehicle Management

EquipmentController, VehicleController

Keep records of equipment and vehicles used in farming.

Likely tracks availability, maintenance, and assignments.

### Logs & Monitoring

LogController, HealthCheckController

Store operation logs (activities, issues, usage).

System health/status checking.

### DTO & Entity Layer

DTOs (AnimalDTO, FieldDTO, VehicleDTO…) for data transfer.

Entities (AnimalEntity, UserEntity, etc.) map to database tables.

### Exception Handling

Custom exceptions (CropNotFoundException, DataPersistException, etc.).

AppWideExceptionHandler (typo in file: AddWideExceptionHandler.java) for global error handling.

### In Summary

This project is meant to:

Provide a secured API for managing an farm business.

Handle users, staff, plants,animals, fields, equipment, and vehicles.

Keep operation logs and perform system checks.

### -----------------------------------------------------------------------------------------------------------------

### 2. Screenshots

### backend
![be.png](screenshots%2Fbe.png)

### frontend
![fe.png](screenshots%2Ffe.png)

### dashboard
![dashboard.png](screenshots%2Fdashboard.png)

### animal and plant managemenet page
![animal and plant management page.png](screenshots%2Fanimal%20and%20plant%20management%20page.png)

### equipment management page
![equipment management page.png](screenshots%2Fequipment%20management%20page.png)

### starf managemnet page
![staf management page.png](screenshots%2Fstaf%20management%20page.png)

### vehicle managemnet page
![vehicle management page.png](screenshots%2Fvehicle%20management%20page.png)

### user managemnet page
![user managemnet page.png](screenshots%2Fuser%20managemnet%20page.png)

### field management page
![filed management page.png](screenshots%2Ffiled%20management%20page.png)

### field management page2
![filed management page2.png](screenshots%2Ffiled%20management%20page2.png)

### field management page3
![field management page3.png](screenshots%2Ffield%20management%20page3.png)

### report generate page
![report genegerate page.png](screenshots%2Freport%20genegerate%20page.png)

### report generate page2
![report generate page2.png](screenshots%2Freport%20generate%20page2.png)


### ---------------------------------------------------------------------------------------------------------

### 3. Setup Instructions

### Reference Documentation

For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/3.3.5/maven-plugin)
* [Create an OCI image](https://docs.spring.io/spring-boot/3.3.5/maven-plugin/build-image.html)
* [Spring Data JPA](https://docs.spring.io/spring-boot/3.3.5/reference/data/sql.html#data.sql.jpa-and-spring-data)
* [Spring Web](https://docs.spring.io/spring-boot/3.3.5/reference/web/servlet.html)

### Guides

The following guides illustrate how to use some features concretely:

* [Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)
* [Accessing data with MySQL](https://spring.io/guides/gs/accessing-data-mysql/)
* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/rest/)

### Maven Parent overrides

Due to Maven's design, elements are inherited from the parent POM to the project POM.
While most of the inheritance is fine, it also inherits unwanted elements like `<license>` and `<developers>` from the
parent.
To prevent this, the project POM contains empty overrides for these elements.
If you manually switch to a different parent and actually want the inheritance, you need to remove those overrides.




