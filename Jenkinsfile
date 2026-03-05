pipeline{
    // agent any
    agent {
        node {
            label 'AGENT-1'
            customWorkspace '/some/other/path'
        }
    }

    stages{
        stage('Build'){
            steps{
                echo 'Building the application'
            }
        }
        stage('Test'){
            steps{
                echo 'Testing the application'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deploying the application'
            }
        }

    }
}