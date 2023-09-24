pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                sh 'npm run'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
