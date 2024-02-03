# Run your Spring Boot application in Docker containers

## Switch to superuser:
```sh
sudo su -
 ```
 ## Install Docker:
 ```sh
 yum install -y docker git maven
 ```
 ## Start Docker service:
```sh
 systemctl start docker
 ```

## Enable Docker service on boot:
```sh
systemctl enable docker
 ```

## Clone a Git repository:
```sh
git clone https://github.com/HaneeshDevops/SpringBootEcommerceApplication.git
 ```
## Navigate to the project directory:
```sh
cd SpringBootEcommerceApplication
 ```
## Build Maven project:
```sh
mvn clean install -DskipTests
 ```
## Create a Dockerfile::
```sh
vi Dockerfile
 ```
## Paste the following in Dockerfile
```sh
FROM openjdk:17
ARG CONTAINER_NAME=ecomapp
ARG IMAGE_NAME=ecomapp
EXPOSE 9090
ADD target/EcommereceApp-rest-0.0.1-SNAPSHOT.jar app.jar
ENTRYPOINT ["java", "-jar", "app.jar"]
