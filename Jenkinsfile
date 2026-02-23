pipeline{
    agent any
    stages{
        stage('Dev stage'){
            steps{
                echo "This is my first job"
            }
        }
        stage('Test stage'){
            steps{
                echo "This is my 2nd job"
            }
        }
        stage('Prod'){
            steps{
                echo "This is the final (prod) job"
            }
        }
    }
    post{
        always{
            echo "Cleaning up resource"
        }
        failure{
            echo " Build failed, sending notification..."
        }
    }
}

