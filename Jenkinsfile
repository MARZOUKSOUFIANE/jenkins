pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy - Staging') {
            steps {
                sh './deploy st
                aging'
                sh './run-smoke-tests'
            }
        }
        stage('Deploy - Production') {
            steps {
                sh './deploy production'
            }
        }   
    }
}
