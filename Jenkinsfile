pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh './mvnw clean package'
            }
        }
        stage('Test') {
            steps {
                sh './mvnw test'
            }
        }
        stage('Deploy') {
            steps {
                slackSend(channel: '#deployment', message: 'La implementación se realizó con éxito')
            }
        }
    }
}
