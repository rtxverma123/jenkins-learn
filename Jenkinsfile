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
        parallel {
            stage('Fluffy tests'){
                steps{
                    echo 'First step'
                    sh 'docker run hello-world'
                }
            }
            stage('Fluffy tests second'){
      steps {
        sh 'sleep 5'
        sh 'echo Success!'
      }
            }
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
