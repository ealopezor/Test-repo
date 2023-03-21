pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo "building..."'
        sh 'mvn compile'
        sh 'echo "finished building"'
      }
    }

    stage('test') {
      steps {
        echo 'Running test...'
        sh 'mvn test'
        sleep 5
        sh 'echo "test finished"'
      }
    }

  }
  environment {
    x = 'x'
  }
}