pipeline{

    agent any

    stages{
        stage("checkout"){
            steps{
                git url: 'https://github.com/apurv9146/Cafe-App.git'
            }
        }

        stage("docker"){
            steps{
                sh 'docker build -t cafe-app .'
                sh 'docker run -d -p 8090:80 cafe-app'
            }
        }
    }

}
