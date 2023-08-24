pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
      args '-u root'
    }
  }
  stages {
    stage ('CHECK VERSION') {
      steps {
        sh 'java -v'
      }
    }
  } post {
    success {
      sh 'echo SUCCESS!!!'
    }
  }
}
