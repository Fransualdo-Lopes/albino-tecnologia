pipeline {
  agent any

  stages {
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
    stage('Test') {
      steps {
        sh 'npm run test -- --passWithNoTests'
      }
    }
    stage('Dev') {
      steps {
        sh 'npm run dev'
      }
    }
  }
}
