pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Production Approval') {
            steps {
                // This pauses the pipeline and waits for a user click
                input message: 'Deploy to Production?', ok: 'Yes, go!'
            }
        }
        stage('Deploy to Prod') {
            steps {
                echo 'Deploying to production servers...'
            }
        }
    }
}
