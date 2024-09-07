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
                //sh 'npm install'
                echo 'Hello install'
            }
        }

        stage("Build"){
            steps{
               
                echo 'Hello build'
            }
        }

        stage('Start') {
            steps {
                //sh 'chmod +x ./node_modules/.bin/nodemon'
                //sh 'npm start'
                echo 'Hello Start'
            }
        }
        
        stage('Check Docker') {
            steps {
                bat 'docker --version'
                echo 'Hello Docker'
            }
        }
       
        stage("Build Image"){
            steps{  
                bat 'docker build -t my-node-app-v1 .'
                echo 'Hello build image'
            }
        }
       
    }
}
