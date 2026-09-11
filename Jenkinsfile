pipeline {
    agent any 
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm 
                echo 'Code checkout complete.'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Starting the Build phase...'
                sh 'echo "Simulating a successful build process!"'
            }
        }

        stage('Test') {
            steps {
                echo 'Running unit tests...'
                // Intentionally breaking the build below
                sh 'cat missing_test_report.txt' 
            }
        }

        stage('Validation') {
            steps {
                echo 'Running security and code quality checks...'
                sh 'echo "Validation complete. Code is safe to deploy!"'
            }
        }
    }
}
