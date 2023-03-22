pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo "building..."'
        sh 'echo "finished building"'
      }
    }

    stage('test') {
      steps {
        echo 'Running test...'
        sleep 5
        sh 'echo "test finished"'
      }
    }

  }
}