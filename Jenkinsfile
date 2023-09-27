pipeline {
    agent any

    stages {
        stage('Checkout git') {
            steps {
                echo 'Pulling...'
                checkout scm
            }
        }

        stage('Testing Maven...') {
            steps {
                sh "mvn --version"
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