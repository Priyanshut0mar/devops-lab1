pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building application...'
                sh 'echo Build completed successfully'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing application...'
                sh 'test -f README.md'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'mkdir -p deploy'
                sh 'cp README.md deploy/'
            }
        }
    }
}
