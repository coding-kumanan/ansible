pipeline {
    agent any
    environment{
        GLOBEL = "globel-env"   //pipeline variable:All the stages can acces this
    }
    stages{
        stage('stage 1'){
            steps{
                sh "env"
                sh "echo stage 1 shell comment"
                sh "echo globel env variable is ${GLOBEL}"
            }
        }
   }
}