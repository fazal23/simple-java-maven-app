pipeline{
    agent any
   
    stages{
        stage('compile-package'){
            steps{
                 withMaven(maven : 'maven_3_6_3'){
                     sh 'echo $workspace'
                     sh 'mvn -f /var/lib/jenkins/workspace/test2/app'
                     sh 'pwd'
                     sh 'mvn -X clean install'
                 }
            }
           
        }
    }
}
