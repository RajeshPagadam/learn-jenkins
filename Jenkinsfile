pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo build'
            }
        }
        stage('Test') {
            steps {
                sh 'echo test'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo deploy'
            }
        }
    }

    post {
    always {
        echo 'sending mail'
        mail bcc: 'test@gmail.com', body: 'test execution completed success', cc: 'pagadamrajesh1@gmal.com', from: '', replyTo: '', subject: '', to: 'pagadamr@gmal.com'
     }
    }
}