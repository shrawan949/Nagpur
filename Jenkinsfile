pipeline{
   agent any
     stages{
       stage('checkout') {
          steps{
              checkout scm
              }}
       stage('BUILD') {
          steps{
              sh 'mvn install'
               }}
       stage('Depolyment') {
          steps{
            sh 'cp /root/.jenkins/workspace/Nagpur/target/Nagpur.war  /root/apache-tomcat-11.0.15/webapps'
               }}

