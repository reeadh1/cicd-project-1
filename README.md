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

- **SCANNER_HOME**: This variable should point to the location of the Sonar Scanner tool in your system.

### Example Configuration

```bash
export SCANNER_HOME=/path/to/sonar-scanner
 
