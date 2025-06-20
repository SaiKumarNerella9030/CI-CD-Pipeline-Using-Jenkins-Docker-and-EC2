pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        checkout scm
      }
    }
    stage('Build Docker Image') {
      steps {
        script {
          docker.build("node-ci-app")
        }
      }
    }
    stage('Run Container') {
      steps {
        script {
          sh 'docker rm -f node-ci-app || true'
          sh 'docker run -d -p 3000:3000 --name node-ci-app node-ci-app'
        }
      }
    }
  }
}
