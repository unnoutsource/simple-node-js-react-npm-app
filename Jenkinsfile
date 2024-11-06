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
        stage('Run Powershell Command (File)') {
            steps {
                echo 'Start Execute'
                script {
                    powershell './myscript.ps1'
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