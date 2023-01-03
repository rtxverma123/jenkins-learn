pipeline {
  agent any
  stages {
    stage('Fluffy Build') {
      parallel {
        stage('Fluffy Build') {
          steps {
            echo 'Placeholder'
            sh 'echo Edited Placeholder.'
            sh 'chmod +x build.sh'
            sh './build.sh'
          }
        }

        stage('fluffy Para') {
          steps {
            echo 'Running parallely'
          }
        }

      }
    }

    stage('Fluffy Test') {
      steps {
        sh 'sleep 5'
        sh 'echo Success!'
      }
    }

    stage('Fluffy Deploy') {
      steps {
        echo 'Placeholder'
      }
    }

  }
  environment {
    BUZZ_NAME = 'Worker Bee'
  }
}