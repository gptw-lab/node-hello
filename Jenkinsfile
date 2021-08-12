pipeline {
  agent {
    docker {
      image 'node:16-alpine3.11'
    }

  }
  stages {
    stage('Print Version') {
      steps {
        sh 'npm -v'
      }
    }

    stage('Build') {
      steps {
        sh 'npm install'
      }
    }

    stage('Run') {
      steps {
        sh 'npm start'
      }
    }

  }
}