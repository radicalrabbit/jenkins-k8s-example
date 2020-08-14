pipeline {  environment {
    registry = "https://github.com/radicalrabbit/jenkins-k8s-example.git"
  }  agent any  stages {
    stage('Building image') {
      steps{
        script {
          docker.build registry + ":$BUILD_NUMBER"
        }
      }
    }
  }
}
