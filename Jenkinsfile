pipeline {
    agent any
    stages {
        stage('SCM Checkoout') {
            steps {
                def mvnHome = tool name: 'apache-maven-3.6.3', type: 'maven'
                sh "${mvnHome}/bin/mvn package"
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
