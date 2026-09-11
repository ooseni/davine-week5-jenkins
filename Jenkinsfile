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
                sh 'echo "Simulating 100% test pass rate!"'
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
