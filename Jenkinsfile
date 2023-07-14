pipeline {
    agent any
    stages {
        stage('Docker Cleanup'){
            steps{
                sh "docker rmi -f $(docker images) || true"
                sh "docker rm -f $(docker ps -aq) || true"

            }
        }
        stage('build app image'){
            steps{
                sh "docker build -t myapp ."
            }
        }
        stage('run app container'){
            steps{
                sh "docker run -d --name myapp myapp"
            }
        }
        
    }
}