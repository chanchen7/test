pipeline {
  agent any
  stages {
    stage('001_中文中文') {
      steps {
        catchError(buildResult: 'FAILURE', stageResult: 'FAILURE', catchInterruptions: true, message: 'TEST') {
          echo 'echo "message"'
          sh 'newman run 001_中文中文.json'
        }

      }
    }
    stage('test3') {
      steps {
        catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
          echo 'echo "message"'
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
