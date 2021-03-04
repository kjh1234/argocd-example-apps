pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        sh 'echo "test"'
        git(url: 'https://github.com/kjh1234/argocd-example-apps.git', branch: 'test', credentialsId: 'GIT_CREDENTIALS_ID')
      }
    }

  }
  environment {
    jenkins = 'file'
    GIT_CREDENTIALS_ID = 'GIT_CREDENTIALS_ID'
  }
}