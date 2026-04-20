pipeline {
    agent any

    environment {
        APP_NAME = "ci-cd-demo"
    }

    stages {

        stage('Build') {
            steps {
                echo "Building ${APP_NAME}"
                sh 'node app.js'
            }
        }

        stage('Test') {
            steps {
                echo "Testing ${APP_NAME}"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying ${APP_NAME}"
            }
        }
    }

    post {
        success {
            echo "Pipeline Success ✅"
        }
        failure {
            echo "Pipeline Failed ❌"
        }
    }
}