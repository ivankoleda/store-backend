pipeline {
  agent {
    docker {
      image 'node:16.13.1-alpine'
    }

  }
  stages {
    stage('install deps') {
      steps {
        sh 'npm ci'
      }
    }

    stage('test') {
      steps {
        sh 'npm run test'
      }
    }

    stage('build') {
      steps {
        sh 'npm run build'
      }
    }

  }
}