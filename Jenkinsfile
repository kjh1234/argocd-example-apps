pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        sh 'echo "test"'
        git(url: 'https://github.com/kjh1234/argocd-example-apps.git', branch: 'test', credentialsId: 'GIT_ID_PW_CREDENTIALS')
      }
    }

  }
  environment {
    jenkins = 'file'
    GIT_ID_PW_CREDENTIALS = 'GIT_ID_PW_CREDENTIALS'
  }
}