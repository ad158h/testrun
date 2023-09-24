pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Get the latest code from the Git repository
                git 'https://github.com/ad158h/testrun.git'
            }
        }
        stage('Build') {
            steps {
                // Build the web application (e.g., using npm, Maven, etc.)
                sh 'npm install'
                sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                // Run tests (e.g., using Jest, Selenium, etc.)
                sh 'npm test'
            }
        }
    }
}
