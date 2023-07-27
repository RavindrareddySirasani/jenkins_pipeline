pipeline {
  agent {
    label 'slave1'
  }
  stages {
    stage('git checkout') {
      steps {
        sh "echo 'this is download git code from github'>file4.txt"
      }
    }
    stage {
      steps {
        echo "build the code"
      }
    }
    stage {
      steps {
        echo "deploy the code"
      }
    }
  }
}
post {
  always {
    echo "all stages are processing"
  }
}
