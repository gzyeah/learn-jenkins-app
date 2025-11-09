pipeline {
    agent {
        label 'docker-with-node'
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
                ls -las
                pwd
                npm start
                '''
            }
        }
    }
}
