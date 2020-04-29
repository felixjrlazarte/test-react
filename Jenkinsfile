pipeline {
    agent {
        docker {
            image 'node:12-alpine
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            environment {
                HOME = '.'
            }
            steps {
                sh 'npm install' 
            }
        }
    }
}