pipeline {
    agent {
        docker {
            image 'node:12-alpine'
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