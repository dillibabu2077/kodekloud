pipeline{
    agent any
     stages{
         stage('mvn clean package'){
             steps{
                sh 'mvn clean package' 
             }
         }
         stage('Docker build'){
             steps{
                sh "docker build -t dillibabun97/hiring:0.0.1"
             }
         }
         stage('Docker Push'){
             steps{
                sh "docker login -u dillibabun97 -p Seenu94@a"
                sh "docker push dillibabun97/hiring:0.0.1" 
             }
         }
     }
}
