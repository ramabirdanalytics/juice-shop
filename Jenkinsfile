pipeline {
  agent {
    docker {
      image 'bkimminich/juice-shop'
      args '-p 3001:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }

    stage('eslint') {
      steps {
        sh 'npm install --save-dev eslint-plugin-security'
      }
    }

    stage('Test with Eslint') {
      steps {
        sh 'npm test'
      }
    }

  }
}