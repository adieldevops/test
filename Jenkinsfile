pipeline {

  agent any

  stages {

    stage('Checkout Source') {
      steps {
        git 'https://github.com/adieldevops/test.git'
      }
    }

    stage('Build image') {
      steps{
        script {
          'docker'
        }
      }
    }

  }

}
