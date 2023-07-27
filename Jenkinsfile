pipeline {
  agent {
    label 'slave2'
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
        sh "echo 'file1 content'>abc.txt"
      }
    }
    stage('input') {
      steps {
        input('do you want to continue?')
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

