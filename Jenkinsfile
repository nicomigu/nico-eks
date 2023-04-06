pipeline {
agent any 
  stages {
    stage('Build eks cluster') {
      steps {
        sh "aws cloudformation create-stack --stack-name nicoKube --template-body file://kubernetes.yaml --region 'us-east-1'"
      }
    }
  }

}