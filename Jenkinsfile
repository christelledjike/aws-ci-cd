pipeline {
    agent any
    }
    environment{
      BRANCH_NAME = 'main'
      GIT_URL = 'https://github.com/christelledjike/aws-ci-cd.git'
      IMAGE_TAG = 'christelledjike/aws-ci-cd'
      IMAGE_VERSION = "${BUILD_NUMBER}"
      }
      stages {
        stage('git checkout') {
            steps {
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }
      stage('docker build'){
           steps{
            sh 'docker build -t awscicd .'
            sh 'docker images'
           } 
        }
    
}
}
