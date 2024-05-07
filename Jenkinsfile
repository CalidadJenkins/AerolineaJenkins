pipeline {
    agent any

    stages {
        stage ('test') {
            steps {
                script {
                    bat 'mvn test'
                }
            }
        }

        stage ('Build') {
            steps {
                script {
                    bat 'mvn -B -DskipTests clean package'
                }
            }
        }
    }
}