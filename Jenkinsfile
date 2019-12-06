pipeline{
    agent any
   
    stages{
        stage('compile-package'){
            steps{
                 withMaven(maven : 'maven_3_6_3'){
                     sh 'pwd'
                     sh 'echo $WORKSPACE'
                     sh 'cd $WORKSPACE/app'
                     
                     sh 'mvn -X clean install'
                 }
            }
           
        }
    }
}
