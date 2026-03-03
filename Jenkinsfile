pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Build Stage'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Script'
                bat 'python app.py'
            }
        }

        stage('Success') {
            steps {
                echo 'Pipeline executed successfully!'
            }
        }
    }
}