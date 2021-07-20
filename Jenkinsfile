pipeline {
  agent {
    docker {
      image 'bkimminich/juice-shop'
      args '-p 3001:3000'
    }

  }
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'npm install'
          }
        }

        stage('eslint') {
          steps {
            sh 'npm install eslint --save-dev'
          }
        }

      }
    }

  }
}