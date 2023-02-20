pipeline {
    agent any

    stages {
        stage('Parallel Execution') {
            steps {
                parallel(
                    a:{
                      echo "Building"
                    },
                    b:{
                        echo "Testing"
                    },
                    c:{
                        echo "Deploying"
                    }
                    )
        stage('Email Build Status') {
            steps {
                mail bcc: '', body: 'Indication of failure', cc: '', from: '', replyTo: '', subject: 'Indication of failure', to: 'gljanani402@gmail.com'
            }
        }    
    }
}
