pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      steps {
        sh 'echo Build stage with $CLOUD_NAME'
      }
    }

    stage('Buzz Test') {
      steps {
        sh 'echo Test Stage with $CLOUD_NAME'
      }
    }

  }
  environment {
    CLOUD_NAME = 'azure'
  }
}