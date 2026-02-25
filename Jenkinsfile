pipeline{
  agent any
  stages{
    stage('clone'){
      steps{
        git banch:'main',url:https:'github.com/satwik500/Calculator.git';
      }
    }
    stage('compile'){
      steps{
        sh 'javac calculator.java'
      }
    }
    stage('build'){
      steps{
        sh 'java calculator 25 5'
      }
    }
  tage('test'){
    steps{
      sh 'java calculator 30 -5'
    }
  }
    stage('Deploy')
    steps {
      echo 'Deployment completed'
    }
  }
}
