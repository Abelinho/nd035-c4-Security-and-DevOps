pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        sh 'checkout([$class: \'GitSCM\', branches: [[name: \'*/master\']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: \'https://github.com/Abelinho/nd035-c4-Security-and-DevOps.git\']]])'
      }
    }

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