pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Building......'
            }
        }
        stage('test') {
            steps {
                echo 'testing......'
            }
        }
        stage('docker') {
            steps {
                docker('docker'){
                sh 'docker build -t app .'
                echo 'deploying......'
            }
            }
        }
        
    }
}
