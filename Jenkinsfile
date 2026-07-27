pipeline {
    agent any

    stages {
        stage('git checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/christelledjike/aws-ci-cd.git'
            }
        }
        stage('test'){
           steps{
            sh 'echo work'
           } 

        }
    }
}