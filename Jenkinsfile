pipeline {
    agent {
        label 'AGENT-1'
    }
    options {
        timeout(time: 30, unit: 'MINUTES')
        disableConcurrentBuilds() 
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo This is build'
            }
        }
        stage('Test') {
            steps {
                sh 'echo This is test'
                sh 'sleep 10'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo This is deploy'
            }
        }
    }
}