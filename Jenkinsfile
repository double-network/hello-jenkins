pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Hello Jenkins') {
      steps {
        echo "Hello ${MY_NAME}!"
        sh 'java -version'
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
      }
    }
  }
  environment {
    TEST_USER = credentials('test-user')
    HER_NAME = 'Mary'
  }
}