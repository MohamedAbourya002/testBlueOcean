pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build completed'
      }
    }

    stage('Test stages') {
      parallel {
        stage('test1') {
          steps {
            echo 'running test1'
            echo 'test'
          }
        }

        stage('test2') {
          steps {
            echo 'run test2'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy completed'
      }
    }

  }
}