pipeline {
    agent any
    stages {
        stage('Run Powershell Command') {
            steps {
                echo 'Start Execute'
                script {
                    powershell '''
                        Write-Output "Hello World"
                        $date = Get-Date
                        Write-Output "Current Date and Time: $date"
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