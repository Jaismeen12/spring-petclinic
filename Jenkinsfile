pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code checkout'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
            }
        }

        stage('Docker Build') {
            steps {
                echo 'Building Docker image'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to Kubernetes'
            }
        }
    }
}