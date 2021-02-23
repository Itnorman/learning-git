# Docker Workshop
Lab 01: First interactions with containers

---

## Instructions

- Pull the jenkins image:

```
$ docker pull ildcworkshops/jenkins
```

 - Check the current running containers and images:
```
$ docker ps
```
```
$ docker images
```

 - Browse to the port 8080 to show to show that it's empty:
```
http://localhost:8080
```

 - Run a Jenkins container
```
$ docker run --name jenkins -p 8080:8080 ildcworkshops/jenkins
```

 - Browse to the Jenkins application
```
http://localhost:8070

```

 - Search for the administrator password in the log:
```
*************************************************************
*************************************************************
*************************************************************  
Jenkins initial setup is required. An admin user has been created and a password generated.
Please use the following password to proceed to installation:  
f7702d8c3e204cf7bfcce76dea9e1ec0  
This may also be found at: /var/jenkins_home/secrets/initialAdminPassword  
*************************************************************
*************************************************************
*************************************************************
```

 - Configure Jenkins using the administration password
 
 - See that Jenkins is up and running
 
 - hit Ctrl+C to exit.
 