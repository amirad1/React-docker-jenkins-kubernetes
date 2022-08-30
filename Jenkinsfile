pipeline {
  agent any
  stages{
    stage('test'){
      steps{
        sh 'cd docker && docker build -t react .'
      }
    }
  }
}
