pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test step'
          }
        }

        stage('test par') {
          steps {
            echo 'test par step'
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
