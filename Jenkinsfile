
pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-u root'
        }
    }
    stages {
        stage('CHECK VERSION'){
            steps{
                sh 'java -version'
            }
        }
    }
    post {
        success {
            sh 'echo BUILD SUCCESS!!!'
        }
    }
}
