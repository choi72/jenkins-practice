pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                sh 'ls -al'
            }
        }

        stage('Build') {
            steps {
                echo 'Build step'
            }
        }

        stage('Deploy to Dev') {
            when {
                branch 'dev'
            }
            steps {
                echo 'Deploying to DEV'
            }
        }

        stage('Deploy to Prod') {
            when {
                branch 'main'
            }
            steps {
                echo 'Deploying to PROD'
            }
        }
    }
}
