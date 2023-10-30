pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello Build'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test job'
          }
        }

        stage('Best') {
          steps {
            echo 'Best'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy Hello'
      }
    }

  }
}