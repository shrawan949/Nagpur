pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh 'mvn install'
            }
        }

        stage('Deployment') {
            steps {
                sh 'cp target/Nagpur.war /root/apache-tomcat-11.0.15/webapps/'
            }
        }
    }
}

