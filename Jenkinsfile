pipeline {
    agent any

    stages {
        stage('Checkout SCM') {
            steps {
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building the code...'
                bat 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running npm audit for security check...'
                bat 'npm audit --json'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy step here (if any)'
                // Put your deploy commands here, using bat if on Windows
            }
        }
    }
}
