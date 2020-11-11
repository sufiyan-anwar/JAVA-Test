pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                ./mvnw -Dmaven.test.failure.ignore=true clean package
            }
        }
        stage('Test') {
            steps {
                mvn test
            }
        }
    }
}
