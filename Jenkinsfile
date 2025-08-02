pipeline{

    agent any

    stages{
        stage("docker"){
            steps{
                sh 'docker build -t cafe-app .'
                sh 'docker run -d -p 8090:80 cafe-app'
            }
        }
    }

}
