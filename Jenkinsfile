pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('parallel') {
          steps {
            echo 'parallel'
          }
        }

      }
    }

    stage('finish') {
      steps {
        echo 'finish'
      }
    }

  }
}