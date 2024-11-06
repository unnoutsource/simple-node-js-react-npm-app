pipeline {
    agent any
    stages {
        stage('Run Powershell Command') {
            steps {
                echo 'Start Execute'
                script {
                    powershell '''
                        C:\\test-script\\myscript.ps1
                    '''
                }
            }
        }
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
    }
}