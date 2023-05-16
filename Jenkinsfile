pipeline{
  agent any
  stages{
    stage("Manage EKS cluster"){
      step{
        sh "eksctl create cluster -f cluster.yaml"
      }
    }
  }
}
