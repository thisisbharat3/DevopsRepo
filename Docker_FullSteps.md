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
git clone https://github.com/thisisbbharat/sample.git
 ```
## Navigate to the project directory:
```sh
cd sample
 ```
## Build Maven project:
```sh
mvn clean install -DskipTests
 ```
## Create a Dockerfile if it is not present in root directory. skip this if Dockerfile exists:
```sh
vi Dockerfile
 ```
## Paste the following in Dockerfile
```sh
FROM openjdk:17
COPY target/sample-v1.jar  sample.jar
EXPOSE 8080
ENTRYPOINT [ "java", "-jar" , "sample.jar" ]"]
```
## docker login
```sh
docker login
```

## Tag image 
```sh
docker tag sample:latest bharathsaho/sample:latest
```
## docker push 
```sh
docker push bharathsaho/sample:latest
```

## see images
```sh
docker images
```

## see running images
```sh
docker ps
```

## see running+stopped images
```sh
docker ps -a
```









