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
               
                echo 'Hello build'
            }
        }

        stage('Start') {
            steps {
                sh 'chmod +x ./node_modules/.bin/nodemon'
                sh 'npm start'
                echo 'Hello Start'
            }
        }
       
        stage("Build Image"){
            steps{  
                echo 'Hello build image'
            }
        }
       
    }
}
