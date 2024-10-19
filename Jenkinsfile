pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add  build steps here, e.g., compile code, run build tools
                sh 'make build' // Example build command
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add test steps here, e.g., run unit tests
                sh 'make test' // Example test command
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add deploy steps here, e.g., deploy to a server
                sh 'make deploy' // Example deploy command
            }
        }
    }

    post {
        always {
            echo 'Cleaning up...'
            // Add any cleanup steps here
            sh 'make clean' // Example cleanup command
        }
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}