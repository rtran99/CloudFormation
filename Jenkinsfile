pipeline {
  agent any
  stages {
    stage('Create CloudFormation Stack') {
      steps {
        script {
          sh "aws cloudformation create-stack --stack-name Ronycloud --template-body file://ec2.yaml --region us-east-1 --capabilities CAPABILITY_IAM"
        }
      }
    }
  }
}
