pipeline{
    // agent any
    agent {
        node {
            label 'AGENT-1'
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

    post { 
        always { 
            echo 'I will always say Hello pipeline!'
        }
        success { 
            echo 'Hello pipeline is success!'
        }
    }
}