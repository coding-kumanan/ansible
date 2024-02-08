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
            }
        }
        stage('running feature'){
        when{branch 'test'}
            steps{
                sh "echo feature branch"
            }
        } 
        stage('running agained pull req'){
        when { branch pattern: "PR-.*", comparator: "REGEXP"}
            steps{
                sh "echo feature branch"
            }
        }
    }
}
//