pipeline {
	agent any

  stages {

    stage('Deploy New Image') {
      steps {
        script {
          kubernetesDeploy(configs: "deployment.yaml", kubeconfigId: "kubeconfig")
        }
      }
    }
  }
}