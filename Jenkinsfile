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
    sh 'npm install'          // install dependencies
    sh 'npm audit --json'     // run npm audit and output JSON (or just `npm audit` if you prefer)
  }
}


    stage('Deploy') {
      steps {
        echo 'Deploying app...'
      }
    }
  }
}
