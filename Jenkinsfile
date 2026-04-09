pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t simple-python-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 5001:5000 simple-python-app'
            }
        }
    }
}