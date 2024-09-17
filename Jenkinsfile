

pipeline {
    agent { label 'NODE2' }
    options {
        timeout(time: 1, unit: 'HOURS')
    }
    triggers {
        pollSCM('* * * * *')
    }
    stages {
        stage('source code') {
            steps {
                git url: 'https://github.com/Prasadsgithub/spring-petclinic.git' ,
                branch: 'main'
            }
        }
        stage('Build the code and sonarqube analysis') {
            steps {
                sh 'mvn package'
            }
        }
    stage('source code') {
        steps {
            git url: 'https://github.com/Prasadsgithub/spring-petclinic.git' ,
            branch: 'main'
        }    
    }
  }
}
    

