pipeline {
  agent {
    docker {
      image 'bkimminich/juice-shop'
      args '-p 3000:3001'
    }

  }
  stages {
    stage('error') {
      steps {
        sh 'npm install'
      }
    }

  }
}