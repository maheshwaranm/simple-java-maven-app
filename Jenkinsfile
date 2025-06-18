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
                echo "This is Build stage"
            }
        }
        stage (test)
        {
            steps
            {
                echo "This is test stage"
            }
        }
        stage (deploy)
        {
            steps
            {
                echo "This is Deploy stage"
            }
        }
    }
}
