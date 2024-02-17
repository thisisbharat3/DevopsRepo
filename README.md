
```
Manage jenkins : Global Tool configuration:
add maven & docker
Add dokcer & docker-compose plugins
New Job:
Name: jenkins_devops_microservice_pipeline
select pipeline option from down


select Poll SCM:* * * * *
go to Pipeline : Pipeline script from SCM
SCM:git & Repository URL : https://github.com/Haneesh55/SpringBootEcommerceApplication.git
BUILD NOW : click on link & openconsole #
```

```
docker rm -f $(docker ps -a)
docker ps -a

docker rm $(docker ps -aq)

docker rmi $(docker images)

bharath
docker tag bharath deepika
docker tag bharath sahobhath/bharath 
docker push sahobharath/bharath


docker stop ID
docker start ID
docker remove ID 

docker pull haneeshdevops/sample

docker start -d -p 8080:8080 haneeshdevops/sample

docker run -d -p 8080:8080 haneshdevops/sample = docker pull haneeshdevops/sample + docker start -d -p 8080:8080 haneeshdevops/sample

docker rm container delete ///// docker rm -f container delete = docker stop ID + docker remove ID 

docker rmi image delete  ///////// docker rmi -f image delete
```
