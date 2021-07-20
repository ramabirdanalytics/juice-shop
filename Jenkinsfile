pipeline {
  agent {
    docker {
      image 'bkimminich/juice-shop'
      args '-p 3000:3000 '
    }

  }
  stages {
    stage('') {
      steps {
        sh 'npm install'
      }
    }

  }
}