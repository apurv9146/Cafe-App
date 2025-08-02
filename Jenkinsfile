pipeline{

    agent any

    stages{
        stage("docker"){
            steps{
                sh 'docker build -t cafe-app .'
                sh 'docker run -d -p 8090:80 cafe-app'
                sh 'docker push 104907335791.dkr.ecr.us-east-1.amazonaws.com/cafe_app'
            }
        }
    }

}
