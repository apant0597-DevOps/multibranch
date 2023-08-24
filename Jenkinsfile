
pipeline {
    agent {
        docker {
            image 'node:16.3.0-alpine'
            args '-u root'
        }
    }
    stages {
        stage('CHECK VERSION'){
            steps{
                sh 'node -v'
            }
        }
    }
    post {
        success {
            sh 'echo BUILD SUCCESS!!!'
        }
    }
}
