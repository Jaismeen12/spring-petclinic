pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Jaismeen12/spring-petclinic.git'
            }
        }

        stage('Build') {
            steps {
                sh 'chmod +x mvnw'
                sh './mvnw clean install'
            }
        }

        stage('Test') {
            steps {
                sh './mvnw test'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t petclinic-app .'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo Deploy step coming soon'
            }
        }
    }
}