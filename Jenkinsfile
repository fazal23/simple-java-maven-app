pipeline{
    agent any
   
    stages{
        stage('compile-package'){
            steps{
                 withMaven(maven : 'maven_3_6_3'){
                     sh 'mvn clean complile'
                 }
            }
           
        }
    }
}
