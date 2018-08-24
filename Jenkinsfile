pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Hello Jenkins') {
      steps {
        echo "Hello ${MY_NAME}!"
        sh 'java -version'
      }
    }
  }
  environment {
    HER_NAME = 'Mary'
  }
}