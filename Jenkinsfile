pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Test') {
            steps {
                mvn test
            }
        }
    }
}
