# Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker
![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/24fb5675-db71-4e19-88eb-44a96c877422)

# Docker is a containerization platform that allows you to package and distribute your applications along with their dependencies. Here's a step-by-step guide to setting up a Docker project for a Spring Boot application:
Install Docker-Desktop.
1. Install Docker:
Ensure that Docker is installed on your machine. You can download and install Docker from the official website: Docker.
2. Create a Spring Boot Application:
If you don't have a Spring Boot application yet, you can create one using Spring Initializr or your preferred method. Include the necessary dependencies for your project.
3. Dockerfile:
Create a Dockerfile in the root of your Spring Boot project. This file contains instructions for building a Docker image for your application. Here's a basic example:
FROM openjdk:11-jre-slim
VOLUME /tmp
ADD target/your-spring-boot-app.jar app.jar
ENTRYPOINT ["java","-jar","/app.jar"]
![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/a3e7c6cd-f09c-444c-8309-b2a1fdc8032c)
Replace your-spring-boot-app with the actual name of your Spring Boot application.
4. Build Docker Image:
Open a terminal in the project directory and run the following command to build the Docker image:
![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/a1047685-1bc2-49b6-8c3b-700f43d62d51)
5. Run Docker Container:
Once the image is built, you can run a Docker container using the following command:
![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/b18bcce7-6202-40fe-a06e-60decbc79c3e)
This command maps port 8080 from the container to port 8080 on your host machine. Adjust the ports as needed.

6. Verify:
Open your web browser and go to http://localhost:8080 to verify that your Spring Boot application is running inside the Docker container.

-------------------------------------------------------------------------------                  ------------------------------------------------------------
![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/8f246ff4-d49c-438a-86a1-0a057e51c862)

# Create Docker Image

![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/f0703470-3a31-473c-a637-bc0afb13136b)
![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/9748498e-3c48-4294-ae9c-075116411758)

# After -SuccessFul
[Docker Images]

![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/7b8f828c-439b-42ef-99e9-18ddfad3cf92)
-------------------------------------------------------


![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/5bb8db1d-1734-437e-8d7a-eef7ae8f2b08)

![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/2c2633f3-da67-4d92-8ea7-c5287f53accb)

-------------------------------------------------------------
 # After You need to setup Mysql New Connection in Mysql WorkBench 3307 from Vm option{before step}

 ![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/838e7e42-6eb7-47c3-9873-37d2fa56bc21)





 
