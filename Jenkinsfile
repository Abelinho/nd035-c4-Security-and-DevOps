pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'sh \'./scripts/build.sh\''
      }
    }

    stage('Test') {
      steps {
        sh 'sh \'./scripts/test.sh\''
      }
    }

    stage('Deploy') {
      steps {
        sh 'sh \'./scripts/deploy.sh\''
      }
    }

  }
}