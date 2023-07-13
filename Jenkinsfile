pipeline {
    agent any
    stages {
        stage('Pipeline stage Build'){
            steps{
                sh "touch build.sh"
                sh 'echo  "stage: Build" > build.sh'
                //sh "chmod +x build.sh"
                //sh "bash build.sh"
            }
        }
        stage('Pipeline stage Test'){
            steps{
                sh "echo stage: Test"
            }
        }
        stage('Pipeline stage Deploy'){
            steps{
                sh "echo stage: Deploy"
            }
        }
        
    }

}