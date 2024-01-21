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
        input(message: 'Are you sure?', ok: 'Yes.')
      }
    }

    stage('Notify') {
      steps {
        echo 'new build completed successfully'
      }
    }

  }
}