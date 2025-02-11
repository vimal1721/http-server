pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'master', url: 'https://github.com/vimal1721/http-server.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }
    }
}
