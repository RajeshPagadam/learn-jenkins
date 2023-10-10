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
        mail bcc: 'pagadamr@gmail.com', body: 'test execution completed success ', cc: 'pagadamr@gmail.com', from: '', replyTo: '', subject: 'test execution', to: 'pagadamr@gmail.com'
     }
    }
}