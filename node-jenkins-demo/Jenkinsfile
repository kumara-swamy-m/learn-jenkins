pipeline {
  agent {
    docker {
      image 'node:16-alpine'
    }
  }

  stages {
    stage('Check Node Version') {
      steps {
        sh 'node --version'
      }
    }

    stage('Install Dependencies') {
      steps {
        sh 'npm install'
      }
    }

    stage('Run App') {
      steps {
        sh 'node app.js'
      }
    }
  }
}
