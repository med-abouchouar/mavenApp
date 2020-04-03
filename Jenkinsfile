pipeline{
    agent any
    tools{
        maven 'Maven 3.6.3'
        jdk 'jdk1.8_231'
     }
     stages{
     stage('build'){
     steps{
     bat 'mvn install'
     }
     post {
     success
     {
     junit 'target/surefire-reports/**/*.xml'
     }
     }
     }
     }
 }
