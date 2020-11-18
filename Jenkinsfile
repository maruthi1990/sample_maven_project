pipeline {
    agent any
    parameters {
        string(name: 'Project', defaultValue: 'Java Project', description: 'Java to deploy on Tomcat Server')
    }
    stages {
        //stage('CleanWorkspace'){
           //steps {
              //cleanWs()
              //sh 'whoami'
           //}
        //}
        stage('Java Webapp Code Pull'){
           steps {
              git branch: 'master', url: 'https://github.com/phani-rudra9/simpe-java-maven-app.git'
           }
        }
        stage('Maven Install package'){
           steps {
              sh 'clean install package'
           }
        }
        
    }    
}		
	
