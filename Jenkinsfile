pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'echo \'Hello Build\''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'echo \'test job\''
          }
        }

        stage('Best') {
          steps {
            echo 'echo \'Best\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'echo \'Deploy Hello\''
      }
    }

  }
}