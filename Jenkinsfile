pipeline {
  agent any
  stages {
    stage('Clone') {
      steps {
        git branch: 'main', url: 'https://github.com/satwik500/Calculator.git'
      }
    }
    stage('Compile') {
      steps {
        sh 'javac calculator.java'
      }
    }
    stage('Build') {
      steps {
        sh 'java calculator 25 5'
      }
    }
    stage('Test') {
      steps {
        sh 'java calculator 30 -5'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deployment completed'
      }
    }
  }
}

