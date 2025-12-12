pipeline {
    agent any
    
    tools {
        maven 'maven-3.9'
        jdk 'jdk-17'
    }
    stages {
        stage('git clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Siva123569/siva.git'
            }
        }
        
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}




