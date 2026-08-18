pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo "Pulling code from GitHub..."
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
                echo "Build stage completed"
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                echo "Test stage completed"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying the project..."
                echo "Deploy stage completed"
            }
        }
    }

    post {
        success {
            echo "CI/CD Pipeline executed successfully!"
        }

        failure {
            echo "CI/CD Pipeline failed!"
        }
    }
}
