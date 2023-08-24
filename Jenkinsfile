pipeline {
  agent {
    docker {
      image 'nginx:1.14.2-alpine'
      args '-u root'
    }
  }
  stages {
    stage ('CHECK VERSION') {
      steps {
        sh 'nginx -v'
      }
    }
  } post {
    success {
      sh 'echo SUCCESS!!!'
    }
  }
}
