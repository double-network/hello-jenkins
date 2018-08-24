pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Hello Jenkins') {
      steps {
        echo 'Hello Jenkins'
        sh 'java -version'
      }
    }
  }
}