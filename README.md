# cicd-project-1
 This project is on spring bot java base project 
### tools part configuration 
 tools {</br>
        jdk 'jdk' </br>
        maven 'mvn'
        } </br>
       
#### first jdk is the tools and second jdk is the name of the tool. this name is given during JDK envrionment setup from Manage Jenkins.

## Environment Setup for sonar scanner tool

To ensure smooth execution of the project, please make sure to set up the following environment variable:

- **SCANNER_HOME**: here we point to sonar scanner home for sonar scanner tools configuration

### Example Configuration

 SCANNER_HOME= tool 'sonar-scanner'

 ## Environment Setup for Sonarqube server credential 
 Keep the sonarqube server credential id as same "sonar-cred" or update jenkinsfile as per your envrionment. 

 ## Environment Setup for docker regestry 
 Keep the docker hub credential id as same "docker-cred" or update jenkinsfile as per your envrionment. 


 ## Environment Setup for Kubernetes credental, namespace and other
 Keep the kubernetes credential id as same "kub-cred" or update jenkinsfile as per your envrionment. </br> Also update namespace as per your environmet
 


## For details document 
https://medium.com/@islamarif/a-cicd-for-java-application-4941ac483345

 
