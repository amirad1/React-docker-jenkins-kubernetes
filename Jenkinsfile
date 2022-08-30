pipeline {
  agent any
  stages{
    stage('Checkout code'){
      steps{
        checkout scm
    }
    }
    stage('test'){
      steps{
        sh '''cd docker
        docker build -t react .'''
      }
    }
    stage('Push image){
          steps{
            sh '''docker tag react amirad1/react:10
            docker push amirad1/react:10'''
      }
    }
  }
}
