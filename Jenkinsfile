pipeline {
  agent any

  environment {
    KUBECONFIG = credentials('kubeconfig-id')
  }

  stages {
    stage('Deploy to Kubernetes') {
      steps {
        sh 'kubectl apply -f k8s-deployment.yaml'
      }
    }
  }
}
