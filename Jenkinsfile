pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the code...'
                // Add any build commands here if needed
            }
        }
        stage('Test') {
            steps {
                echo 'Running npm audit for security check...'
                bat 'npm install'
                bat 'npm audit --json'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add deploy commands here
            }
        }
    }
}
