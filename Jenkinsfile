pipeline{
 agent {
     docker { 
         image "papitoio/node-wd",
         args "--network=skynet"
         
         }
 }  
 stages {
     stage('Build') {
         steps{
            sh "npm install"

         }
          
     }
     stage('Tests') {
         steps {
            sh "npm test: ci"
         }
         
     }
 }
}