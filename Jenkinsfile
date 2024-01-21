pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Completed '
      }
    }

    stage('Test2') {
      parallel {
        stage('Test stages') {
          steps {
            echo 'running test2'
          }
        }

        stage('TEST 1') {
          steps {
            echo 'RUNNING TEST1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment Completed'
      }
    }

  }
}