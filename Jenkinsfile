pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'sh \'mvn clean install\''
      }
    }

    stage('Test') {
      steps {
        sh 'sh \'mvn test\''
      }
    }

    stage('Deploy') {
      steps {
        sh 'sh \'mvn spring-boot:run\''
      }
    }

  }
}