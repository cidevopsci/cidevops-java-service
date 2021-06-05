pipeline {
  agent {
    node {
      label 'build'
    }

  }
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'Hello World!'
          }
        }

        stage('linux build') {
          steps {
            echo 'Linux build'
          }
        }

        stage('win build') {
          steps {
            echo 'win build'
          }
        }

      }
    }

  }
  environment {
    VERSION = '1.1.1'
  }
}