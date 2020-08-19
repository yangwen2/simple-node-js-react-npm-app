pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000 --dns 8.8.8.8' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}