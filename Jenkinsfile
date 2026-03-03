pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps { checkout scm }
    }
    stage('Run in Docker') {
      steps {
        bat 'docker run --rm -v "%cd%":/app -w /app python:3.11 python app.py'
      }
    }
  }
}