pipeline {
    agent any
    stages{
        stage("checkout"){
            steps{
                checkout scm
                echo 'Hello checkoutl'
            }
        }

        stage("Test"){
            steps{
                sh 'npm install'
                echo 'Hello install'
            }
        }

        stage("Build"){
            steps{
                sh 'npm run build'
                echo 'Hello build'
            }
        }

        stage("Build Image"){
            steps{  
                echo 'Hello build image'
            }
        }
       
    }
}
