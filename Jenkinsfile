pipeline {
    agent { label 'agent-1' }

    stages {
        stage('Checkout Confirm') {
            steps {
                echo 'Checked out from SCM successfully.'
                sh 'pwd'
                sh 'ls -la'
            }
        }
        stage('Hello') {
            steps {
                sh 'hostname'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'
        }
    }
}
