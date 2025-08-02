pipeline{

    agent any

    stages{
        stage("docker"){
            steps{
                sh 'docker build -t cafe-app .'
                sh 'docker tag cafe_app:latest 104907335791.dkr.ecr.us-east-1.amazonaws.com/cafe_app:latest'
                sh 'docker push 104907335791.dkr.ecr.us-east-1.amazonaws.com/cafe_app:latest'
            }
        }
    }

}
