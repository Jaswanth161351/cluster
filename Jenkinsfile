pipeline {
  agent any
  environment {
    AWS_REGION = 'ap-south-1'
  }
  stages {
    stage('Create EKS cluster') {
      steps {
        withCredentials([[
          $class: 'AmazonWebServicesCredentialsBinding',
          accessKeyVariable: 'AKIA444LDZJOKF7Q2A4O',
          secretKeyVariable: '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'
        ]]) {
          sh 'eksctl create cluster --name my-cluster --version 1.21 --region ${AWS_REGION} --nodegroup-name my-node-group --node-type t3.small --nodes 3'
        }
      }
    }
  }
}
