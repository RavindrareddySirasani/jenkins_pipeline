pipeline {
  agent {
    label 'slave1'
  }
  stages {
    stage('git checkout') {
      steps {
        echo 'this is download git code from github'
      }
    }
    stage('build') {
      steps {
        echo "build the code"
      }
    }
    stage('deploy') {
      steps {
        echo "deploy the code"
      }
    }
  }
  post {
    success {
      echo "all stages are processing"
    }
  }
}

