pipeline {
    agent {
        node { label 'nodejs' }
    }
    stages {
        stage("Clone and Install Packages") {
            steps {
                nvm('8.11.3') {
                    echo "Cloning info..."
                    sh 'npm install'
                }
            }
        }
        stage("Unit Test") {
            steps {
                nvm('8.11.3') {
                    sh 'npm test -- --coverage'
                }
            }
        }
    }
}