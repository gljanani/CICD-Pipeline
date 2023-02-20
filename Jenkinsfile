pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('Email Build Status') {
            steps {
                mail bcc: '', body: 'Indication of failure', cc: '', from: '', replyTo: '', subject: 'Indication of failure', to: 'gljanani402@gmail.com'
            }
        }    
    }
}
