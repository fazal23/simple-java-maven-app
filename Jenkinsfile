pipeline{
    agent any
   
    stages{
       stage('Git clone'){
           git'https://github.com/fazal23/simple-java-maven-app'
       }
       stage('compile-package'){
          steps{
              withMaven(maven : 'maven_3_6_3'){
                  sh 'mvn clean complile'
              }
          }
           
       }
    }
}
