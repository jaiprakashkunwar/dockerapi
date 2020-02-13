# dockerapi
#Create Docker API project

1>Open VS code in terminal
dotnet new webapi -n DockerApi

2>Type below ommand to open project in VS code
code -r DockerApi

3>build the project 
dotnet build

4>run the app
dotnet run

5>api values:
http://localhost:5000/api/values

6>Build docker image
docker build -t jaiprakashkunwar/dockerapi .

7> docker run
docker run -p 8080:80 jaiprakashkunwar/dockerapi

8> press ctrl+c to terminate the container but still container is running. you can verify this
docker ps
this will give you containerid

9> stop container 
docker stop <containerid>

10>push to dockerhub

docker push jaiprakashkunwar/dockerapi

*************************************************Deploying on Azure***************************************
1>Go to azure portal
 creaete resource-->create container instance
 networking--> put DNS name
