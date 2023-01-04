pipeline {
  agent any
  stages {
    stage('Gitpull') {
      parallel {
        stage('Gitpull') {
          steps {
            sh 'echo "Pulling application"'
          }
        }

        stage('Unit Testing') {
          steps {
            sh 'echo "Unit Testing"'
          }
        }

      }
    }

    stage('Bulid') {
      steps {
        sh 'echo "BUild Application"'
      }
    }

    stage('Deploy-to-prod') {
      steps {
        sh 'echo "Deploy to production"'
      }
    }

  }
}