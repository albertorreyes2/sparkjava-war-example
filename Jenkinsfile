pipeline {
    agent { label 'gustavo' }
    stages {
        stage('Build') {
            steps {
                sh '''
                echo "Do something"
                pwd
                uname
                docker ps
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Do something 2"
            }
        }
        stage('Deploy') {
            steps {
                echo "Do something 3"
            }
        }
    }
}
