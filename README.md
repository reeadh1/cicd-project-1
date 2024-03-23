# cicd-project-1
 This project is on spring bot java base project 
### tools part configuration 
 tools {</br>
        jdk 'jdk' </br>
        maven 'mvn'
        } </br>
       
#### first jdk is the tools and second jdk is the name of the tool. this name is given during JDK envrionment setup from Manage Jenkins.

## Environment Setup

To ensure smooth execution of the project, please make sure to set up the following environment variable:

- **SCANNER_HOME**: here we point to sonar scanner home for sonar scanner tools configuration

### Example Configuration

```bash
 SCANNER_HOME= tool 'sonar-scanner'

## Environment Setup

To ensure smooth execution of the project, please make sure to set up the following environment variable:

- **DOCKER_REGISTRY_CREDENTIALS**: This variable should be set with the credentials ID for accessing the Docker registry. in my case "docker-cred" if you want to use this pipline keep the name same or update you jenkins file as per you environment.

### Example Configuration

```bash
DOCKER_REGISTRY_CREDENTIALS=docker-cred



 
