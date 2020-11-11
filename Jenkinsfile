pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                def mvnHome = tool name: 'Maven 3.6.3', type: 'maven'
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
