pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo "Code already checked out by Jenkins"
                sh 'ls -l'   // just to verify files exist
            }
        }
        stage('Build') {
            steps {
                echo "Building project..."
                sh 'echo "Build successful!"'
            }
        }
        stage('Test') {
            steps {
                echo "Running tests..."
                sh 'echo "All tests passed!"'
            }
        }
    }
    post {
        success {
            echo "Pipeline executed successfully."
        }
        failure {
            echo "Pipeline failed!"
        }
    }
}
