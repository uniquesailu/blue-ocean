pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo \'Building\''
      }
    }

    stage('test') {
      steps {
        sh 'echo \'Testing\''
      }
    }

    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            sh 'echo \'Deploying\''
          }
        }

        stage('Deploy2') {
          steps {
            echo 'deploy2'
          }
        }

      }
    }

  }
}