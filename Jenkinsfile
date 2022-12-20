pipeline{
    agent any
    stages{
        stage("One"){
            steps{
                echo "========executing One========"
            }
            post{
                always{
                    echo "========always========"
                }
                success{
                    echo "========One executed successfully========"
                }
                failure{
                    echo "========One execution failed========"
                }
            }
        }
        stage("Two"){
            steps{
                echo "====++++executing Two++++===="
            }
            post{
                always{
                    echo "====++++always++++===="
                }
                success{
                    echo "====++++Two executed successfully++++===="
                }
                failure{
                    echo "====++++Two execution failed++++===="
                }
        
            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}