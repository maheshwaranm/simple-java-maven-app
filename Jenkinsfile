pipeline {
    agent
    {
        label 'devserver'
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
