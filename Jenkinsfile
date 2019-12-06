pipeline{
    agent any
   
    stages{
        stage('compile-package'){
            steps{
                 withMaven(maven : 'maven_3_6_3'){
                     sh 'pwd'
                     sh 'echo $WORKSPACE'
                     sh 'mvn -f $WORKSPACE/app clean install'
                     
                     
                 }
            }
           
        }
    }
}
