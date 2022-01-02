pipeline {
    agent { docker { image 'node:16.13.1-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'npm i'
                sh 'npm build'
            }
        }
        stage('test') {
            steps {
                sh 'npm test'
            }
        }
    }
}