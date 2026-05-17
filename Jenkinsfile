pipeline {
    agent any

    environment {
        DOCKER_IMAGE = "arumugam/self-healing-platform"
    }

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/Arumugamthangavel/Self-Healing-Deployment-Platform.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t $DOCKER_IMAGE .'
            }
        }

        stage('Docker Image Verification') {
            steps {
                sh 'docker images'
            }
        }

        stage('Push Docker Image') {
            steps {
                echo 'DockerHub push will be configured later'
            }
        }

        stage('Kubernetes Deployment') {
            steps {
                echo 'Kubernetes deployment phase under development'
            }
        }

    }

    post {
        success {
            echo 'Pipeline executed successfully'
        }

        failure {
            echo 'Pipeline execution failed'
        }
    }
}
