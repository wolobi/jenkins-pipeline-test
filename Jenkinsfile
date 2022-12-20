pipeline{
    agent any
    stages{
        stage("One"){
            steps{
                echo "========Echo One========"
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
                echo "====++++Echo Two++++===="
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
        stage("Three"){
            steps{
                input('¿Quieres proceder con el despliegue?')
            }
            post{
                always{
                    echo "====++++USER INPUT INFO++++===="
                }
                success{
                    echo "====++++Three executed successfully++++===="
                }
                failure{
                    echo "====++++Three execution failed++++===="
                }
        
            }
        }
        stage("Four"){
            steps{
                echo "Desplegando aplicación"
            }
            post{
                always{
                    echo "====++++Despliegue INFO++++===="
                }
                success{
                    echo "====++++Despliegue executed successfully++++===="
                }
                failure{
                    echo "====++++Despliegue execution failed++++===="
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