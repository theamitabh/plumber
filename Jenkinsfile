pipeline {
  agent any
  stages {
    stage(' Build') {
      steps {
        sh 'echo Build stage with $CLOUD_NAME'
      }
    }

    stage('Test in AZ') {
      parallel {
        stage('Test 1') {
          steps {
            sh 'echo Test Stage with $CLOUD_NAME'
          }
        }

        stage('Test in GCP') {
          steps {
            echo 'Google testing going on.....'
          }
        }

      }
    }

  }
  environment {
    CLOUD_NAME = 'azure'
  }
}