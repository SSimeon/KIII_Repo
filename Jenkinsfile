pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repository...'
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                echo 'Building Docker image...'
                sh 'docker build -t simple-docker-image .'
            }
        }

        stage('Done') {
            steps {
                echo 'Pipeline completed.'
            }
        }
    }
}
