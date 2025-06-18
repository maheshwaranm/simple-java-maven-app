pipeline {
    agent
    {
        label 'devserver'
    }
    tools{
        maven 'myMaven'
    }

    stages {
        stage (build)
        {
            steps
            {
                sh 'mvn clean pacakge'
            }
            post{
            success {
                archiveArtifacts artifacts: '**/target/*.war'
            }        
            }
        }
        
    }
}
