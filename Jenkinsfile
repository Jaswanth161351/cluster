pipeline{
  agent any
  stages{
    stage("Manage EKS cluster"){
      steps{
        sh "eksctl create cluster -f cluster.yaml"
      }
    }
  }
}
