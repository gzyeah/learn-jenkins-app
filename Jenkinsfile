pipeline {
    agent {
        docker {
            image 'node:18-alpine'
        }
    }
    stages {
        stage('Stage 1') {
            steps {
                sh '''
                echo hello
                hostname
                '''
            }
        }
        stage('Stage 2') {
            steps {
                sh '''
                ls -la
                node --version
                npm --version
                npm ci
                npm run build
                ls -la
                '''
            }
        }
    }
}
