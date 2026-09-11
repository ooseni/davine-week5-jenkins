pipeline {
    agent any // Tells Jenkins to run this on any available executor/node
    
    stages {
        stage('Checkout') {
            steps {
                // This built-in command securely pulls your code from GitHub 
                // using the credentials we configure in the Jenkins UI
                checkout scm 
                echo 'Code checkout complete.'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Starting the Build phase...'
                // You can run any shell commands here (like docker build or npm install)
                sh 'echo "Simulating a successful build process!"'
                sh 'ls -la'
            }
        }
    }
}
