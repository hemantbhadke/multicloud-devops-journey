pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code already checked out by Jenkins automatically'
                sh 'ls -la'
            }
        }
        stage('Build') {
            steps {
                echo 'Pretending to build the project...'
                sh 'echo "Build step ran at: $(date)"'
            }
        }
        stage('Test') {
            steps {
                echo 'Pretending to run tests...'
                sh 'echo "Test step ran at: $(date)"'
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed — check the logs above.'
        }
    }
}
