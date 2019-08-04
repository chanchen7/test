pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        catchError(buildResult: 'FAILURE', stageResult: 'FAILURE', catchInterruptions: true, message: 'TEST') {
          echo 'echo "message"'
          sh './test'
        }

      }
    }
    stage('test2') {
      steps {
        catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
          echo 'echo "message"'
        }

      }
    }
  }
}