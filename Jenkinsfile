pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'echo "message"'
        sh './test'
      }
    }
    stage('test2') {
      steps {
        sh './test.ps'
      }
    }
  }
}