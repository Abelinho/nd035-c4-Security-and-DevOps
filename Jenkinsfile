pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh './starter_code/build.sh'
      }
    }

    stage('Test') {
      steps {
        sh './starter_code/test.sh'
      }
    }

    stage('Deploy') {
      steps {
        sh './starter_code/deploy.sh'
      }
    }

  }
}