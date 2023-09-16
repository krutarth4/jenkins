pipeline {
  agent any
  stages {
    stage('Bild') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test step'
          }
        }

        stage('test parallel') {
          steps {
            echo 'parallel step'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}