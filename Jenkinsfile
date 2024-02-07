pipeline {
    agent any

    environment {         // Pipeline Variables : All the stages of the pipeline can use it.
        SSH_CRED = credentials('SSH_CRED')
    }
    stages{
        stage('Performing a dry run') {  // This stage should only run when you raise a PULL Request.
            steps {
                sh '''
                    env 
                
                '''
            }
        }
    }
}
