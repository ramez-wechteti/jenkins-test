pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Display Date') {
            steps {
                script {
                    def currentDate = sh(script: 'date', returnStdout: true).trim()
                    echo "Date systeme actuellement est : $currentDate"
                }
            }
        }
    }
}