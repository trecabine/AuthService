# Auth Service

This Web API is built using ASP.NET core 1.0.0.

The purpose of this service is to produce JWT token, enabling to get the token and use the token to authenticate to any other services using the same signing key.


## Overview

* It's using SQL Server as the database server 
* This service is using EntiyFrameworkCore Identity, authenticate against the AspNetUsers.
* This service can be run on Mac or Windows.


## Setting up your machine

Go to the root folder of this service code and run the command below:
```
dotnet restore
```
and then
```
dotnet build
```


## To run this service

### To run this service locally using the terminal (Mac) or powershell (Windows)

Go to the root folder of this service code and run the command below:
```
dotnet run
```

### Using Docker

Go to the root folder of this service code and run the command below:
```
docker build . -t authservice:latest
````
The command above is to build the docker image on your local machine.

Once the image is built then you can run the docker
```
docker run  -d -p 5000:5000 authservice
```


FINALLY, managed to make this running. Republish this service and made the repo to public and open source to utilize free Travis CI