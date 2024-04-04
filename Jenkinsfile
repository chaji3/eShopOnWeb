pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build '
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('test fn') {
          steps {
            echo 'test fn'
          }
        }

        stage('test u') {
          steps {
            echo 'test u'
          }
        }

      }
    }

    stage('deployment') {
      steps {
        echo 'deployement'
      }
    }

  }
}