pipeline {
    agent any
    stages {
        stage('git checkout') {
            steps {
                git branch: "main", url: 'https://github.com/all-projects-files/js-e2e-express-server.git'
            }
        }
        stage('build') {
            steps {
                sh 'npm install'
            }
        }
        stage('start') {
            steps {
                sh 'npm start'
            }
        }
    }
}