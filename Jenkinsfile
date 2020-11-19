pipeline {
    agent any
    parameters {
        string(name: 'Project', defaultValue: 'Java Project', description: 'Java to deploy on Tomcat Server')
    }
    stages {
        stage('Java Webapp Code Pull'){
           steps {
              git branch: 'main', url: 'https://github.com/maruthi1990/sample_maven_project.git'
           }
        }
        stage('Maven Install package'){
          steps {
             sh 'clean install package'
           }
        }
        
    }    
}		
	
