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
 
Infrastructure Preparation:
Assume You have already prepared the following environment.

Jenkins:
You have Jenkins on Docker Or VM or Cloud
2. Docker:
Docker package should be install on Jenkins VM

3. Kubernetes:
You have already prepared your Kubernetes cluster on your environment or cloud.

4. SonarQube:
You can prepare your sonarQube on Docker or VM.

Install Jenkins On ubuntu

Create a script with the following. Create file name jenkins.sh and pest the following code.

#!/bin/bash
# Install OpenJDK 17 JRE Headless
sudo apt install openjdk-17-jre-headless -y
# Download Jenkins GPG key
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
# Add Jenkins repository to package manager sources
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
/etc/apt/sources.list.d/jenkins.list > /dev/null
# Update package manager repositories
sudo apt-get update
# Install Jenkins
sudo apt-get install jenkins -y
SonarQube on Docker:

docker run -d - name sonar -p 9000:9000 sonarqube:lts-community
Configure Jenkins for this Pipeline:
Jenkins Plugin we need:
1. Eclipse Temurin Installer
2. Pipeline Maven Integration
3. SonarQube Scanner
4. Kubernetes CLI
5. Kubernetes
6. Docker
7. Docker Pipeline Step

Configure JDK and Maven on Jenkins
We will configure JDK with automatic installation feature on Jenkins. We will chose jdk 17 or above version. Follow this guide line. Go to Manage Jenkins > Tools > JDK installations > Name your jdk and select Automatically Install option > From dropdown select any version of JDK17
 



 
