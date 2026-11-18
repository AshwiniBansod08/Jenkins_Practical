
pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application'
                sh ' Build Successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing application'
                sh 'test -f index.html'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application'
                sh 'echo Application Deployed Successfully'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }

        failure {
            echo 'Pipeline failed!'
        }
    }
}

