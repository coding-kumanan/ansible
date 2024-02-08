pipeline {
    agent any
    environment{
        GLOBEL = "globel-env"   //pipeline variable:All the stages can acces this
    }
    stages{
    
        stage('running main branch'){
        when{branch 'main'}
            steps{
                sh "env"
                sh "echo stage 1 main"
        when{branch 'test'}
            steps{
                sh 'running test'
            }
            }
        }
   }
}
//