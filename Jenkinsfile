pipeline {
  agent any
  stages {
    stage(' Build') {
      steps {
        sh 'echo Build stage with $CLOUD_NAME'
      }
    }

    stage('Test 1') {
      parallel {
        stage('Test 1') {
          steps {
            sh 'echo Test Stage with $CLOUD_NAME'
          }
        }

        stage('Test 2') {
          steps {
            echo 'Testing Parallel stages'
          }
        }

      }
    }

  }
  environment {
    CLOUD_NAME = 'azure'
  }
}