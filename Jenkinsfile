pipeline {
    agent any
    environment {
        CI = 'true' 
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Test'){
            steps{
                bat 'chmod +x ./jenkins/scripts/test.sh && ./jenkins/scripts/test.sh'
            }
        }
    }
}
