pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/krishn1250/HELLO.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean install'  // If you're using Maven for building the project
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'  // Running tests if available
            }
        }
    }
    post {
        success {
            echo 'Build and tests passed!'
        }
        failure {
            echo 'Build or tests failed.'
        }
    }
}
