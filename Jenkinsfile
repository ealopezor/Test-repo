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

    stage('Exec') {
      steps {
        echo 'Executing'
      }
    }

    stage('Package') {
      steps {
        echo 'Package'
      }
    }

    stage('Manual approval') {
      steps {
        input(message: 'Do you want to deploy?', ok: 'Yes, lets do it', id: 'id', submitter: 'submitter', submitterParameter: 'submitterParameter')
      }
    }

  }
}