pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        echo 'Building the code...'
      }
    }

   stage('Test') {
  steps {
    echo 'Running npm audit for security check...'
    bat 'npm install'          // install dependencies
    bat 'npm audit --json'     // run npm audit and output JSON (or just `npm audit` if you prefer)
  }
}


    stage('Deploy') {
      steps {
        echo 'Deploying app...'
      }
    }
  }
}
