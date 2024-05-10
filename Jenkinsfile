pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat './mvnw clean package'
            }
        }
        stage('Test') {
            steps {
                bat './mvnw test'
            }
        }
    }
}
