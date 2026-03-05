pipeline{
    // agent any
    agent {
        node {
            label 'AGENT-1'
        }
    }
    environment{
        COURSE = 'jenkins'
    }
    options {
        timeout(time: 10, unit: 'SECONDS')
        disableConcurrentBuilds()
    }
   
   // Build
    stages{
        stage('Build'){
            steps{
                script{
                    sh """
                        echo 'Building the application'
                        env
                    """
                    
                }
            }
        }
        stage('Test'){
            steps{
                script{
                    echo 'Testing the application'
                }
            }
        }
        stage('Deploy'){
            steps{
                script{
                    echo 'Deploying the application'
                }
            }
        }

    }

   // Post Build
    post { 
        always { 
            echo 'I will always say Hello pipeline!'
            deleteDir()
        }
        success { 
            echo 'Hello pipeline is success!'
        }
        failure { 
            echo 'Hello pipeline is failure!'
        }
    }
}