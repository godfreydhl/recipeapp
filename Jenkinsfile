pipeline {
    agent any 
    
    stages {
        stage('checkout') {
            steps {
                checkout scm
            }
        }
        stage('Test') {
            steps {
                sh 'sudo apt-get install npm -y'
                sh 'npm test'
            }
        }
        stage('Build') {
            steps {
                sh 'npm build'
            }
        }
    }
}
