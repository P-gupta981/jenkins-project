
       pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t python-jenkins-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run --rm python-jenkins-app'
            }
        }
    }
}
