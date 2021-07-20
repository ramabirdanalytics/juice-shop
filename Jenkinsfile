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

  }
}