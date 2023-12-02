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

![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/12767a55-20f2-420c-83a7-24413c71e4ca)

![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/026c6bf0-79cd-4e09-a504-1c2586fadc55)

![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/dbcf77fc-3987-4a05-a45c-672225a74ae7)


![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/59179f01-6f14-467b-9e47-084bdb20b13a)


After You can Run MVN-Install command in maven

 ![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/69c88179-a9f6-4d26-85c6-a8012f347a63)

![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/1c6f7120-533b-4731-abc6-aa841d7b6d55)

After Command in your Terminal 
 # docker build -t springboot-mysql-docker .


![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/f4553246-40a5-4b8c-9dd0-9552ce89635f)
-------------------------------------
if(Successful==true)--> 😀
---------------------------------
PS E:\Docker\SpringBootMYSQLDocker\SpringBootMYSQLDocker> docker build -t springboot-mysql-docker .
[+] Building 29.0s (8/8) FINISHED                                                                                                                                      docker:default
 => [internal] load .dockerignore                                                                                                                                                0.0s
 => => transferring context: 2B                                                                                                                                                  0.0s
 => [internal] load build definition from Dockerfile                                                                                                                             0.0s
 => => transferring dockerfile: 178B                                                                                                                                             0.0s
 => [internal] load metadata for docker.io/library/openjdk:17                                                                                                                    2.1s
 => [auth] library/openjdk:pull token for registry-1.docker.io                                                                                                                   0.0s
 => [internal] load build context                                                                                                                                                8.0s
 => => transferring context: 42.07MB                                                                                                                                             8.0s
 => [1/2] FROM docker.io/library/openjdk:17@sha256:528707081fdb9562eb819128a9f85ae7fe000e2fbaeaf9f87662e7b3f38cb7d8                                                             26.0s
 => => resolve docker.io/library/openjdk:17@sha256:528707081fdb9562eb819128a9f85ae7fe000e2fbaeaf9f87662e7b3f38cb7d8                                                              0.0s
 => => sha256:528707081fdb9562eb819128a9f85ae7fe000e2fbaeaf9f87662e7b3f38cb7d8 1.04kB / 1.04kB                                                                                   0.0s
 => => sha256:98f0304b3a3b7c12ce641177a99d1f3be56f532473a528fda38d53d519cafb13 954B / 954B                                                                                       0.0s
 => => sha256:5e28ba2b4cdb3a7c3bd0ee2e635a5f6481682b77eabf8b51a17ea8bfe1c05697 4.45kB / 4.45kB                                                                                   0.0s
 => => sha256:38a980f2cc8accf69c23deae6743d42a87eb34a54f02396f3fcfd7c2d06e2c5b 42.11MB / 42.11MB                                                                                 9.1s
 => => sha256:de849f1cfbe60b1c06a1db83a3129ab0ea397c4852b98e3e4300b12ee57ba111 13.53MB / 13.53MB                                                                                 3.9s 
 => => sha256:a7203ca35e75e068651c9907d659adc721dba823441b78639fde66fc988f042f 187.53MB / 187.53MB                                                                              19.3s 
 => => extracting sha256:38a980f2cc8accf69c23deae6743d42a87eb34a54f02396f3fcfd7c2d06e2c5b                                                                                        6.9s
 => => extracting sha256:de849f1cfbe60b1c06a1db83a3129ab0ea397c4852b98e3e4300b12ee57ba111                                                                                        1.2s
 => => extracting sha256:a7203ca35e75e068651c9907d659adc721dba823441b78639fde66fc988f042f                                                                                        6.4s
 => [2/2] ADD target/springboot-mysql-docker.jar springboot-mysql-docker.jar                                                                                                     0.5s
 => exporting to image                                                                                                                                                           0.3s
 => => exporting layers                                                                                                                                                          0.3s
 => => writing image sha256:f962ad205cb45603906ef7b0461c3d260972e6ba5235adfc38162e516f656917                                                                                     0.0s 
 => => naming to docker.io/library/springboot-mysql-docker                                                                                                                       0.0s 

What's Next?
  View a summary of image vulnerabilities and recommendations → docker scout quickview

![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/a3a8736d-464f-42b1-a522-4f0030ec509e)


![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/5bc0f14e-e5c5-44ab-b6e6-b576e649ce23)

![image](https://github.com/PrabhaWijera/Spring-Boot-CRUD-Project-With-MySQL-Database-in-Docker/assets/106425954/c2dab11a-bbb7-4396-88d0-3c15c9e3252e)
