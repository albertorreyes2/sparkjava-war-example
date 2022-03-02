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
                mvn clean install
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
                sh '''
                echo "Do something 3"
                docker cp /root/workspace/gustavoFolder/gustavoPipelinetarget/sparkjava-hello-world-1.0.war tomcat://usr/local/tomcat/webapps 
                echo 'cp do'
                '''
            }
        }
    }
}
