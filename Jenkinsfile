pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning project from GitHub...'
                git branch: 'main', url: 'https://github.com/hogadevedant1212-bit/Jenkin_with_HTML.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Build Step: Checking files in workspace'
            }
        }
        stage('Test') {
            steps {
                echo 'Test Step: Validating HTML (basic check)'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy Step: Files ready for deployment'
            }
        }
    }
    post {
        success {
            echo 'Pipeline finished successfully!'
        }
        failure {
            echo 'Pipeline failed! Check logs.'
        }
    }
}
