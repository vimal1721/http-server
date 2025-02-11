pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'master', url: 'https://github.com/vimal1721/http-server.git'
            }
        }
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t my-web-server .'
            }
        }
        stage('Run Container') {
            steps {
                sh 'docker run -d -p 5000:5000 --name webserver my-web-server'
            }
        }
    }
}

