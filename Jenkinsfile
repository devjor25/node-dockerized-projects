pipeline {
    agent any
    stages{
        stage("checkout"){
            steps{
                checkout scm
            }
        }

        stage("Test"){
            steps{
                sh 'install npm' 
                echo 'Hello test'
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
                sh 'docker build -t my-node-app:2.0 .'
                echo 'Hello build image'
            }
        }
       
    }
}
