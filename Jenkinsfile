Pipeline{
    agent any

    stages{
       stage('Compile Stage'){
       steps{
       withMaven(maven : Maven_Install){
             sh 'mvn clean compile'
             }
           }
        }
       stage('Testing Stage'){
       steps{
       withMaven(maven : Maven_Install){
             sh 'mvn test'
             }
           }
        }
       stage('Deployment Stage'){
       steps{
       withMaven(maven : Maven_Install){
             sh 'mvn deploy'
             }
           }
        } 
       }
       }
       

   
