pipeline{
  agent any
  stages{
    stage("Manage EKS cluster"){
      steps{
        withCredentials([
          [$class: 'AmazonWebServicesCredentialsBinding', 
          credentialsId: 'AWSCredentials'
          AccessKeyVeriable: 'AKIA444LDZJOKF7Q2A4O',
          SecretKeyVariable: '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']])
        sh "eksctl create cluster -f cluster.yaml"
      }
    }
  }
}
