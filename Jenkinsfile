pipeline {
    agent any
    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/krishn1250/HELLO.git'
            }
        }
        stage('Build') {
            steps {
                echo "✅ Building the project..."
                // sh './gradlew build' OR 'mvn clean install' based on your project
            }
        }
        stage('Test') {
            steps {
                echo "🧪 Running tests..."
                // sh './gradlew test'
            }
        }
    }
}
