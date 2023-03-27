pipeline {
  agent any

  stages {
    stage('Install dependencies') {
      steps {
        sh 'npm install'
        sh 'npm install jest --save-dev'
      }
    }
    stage('Test') {
      steps {
        sh 'npm run test -- --passWithNoTests'
      }
    }
  }
}
