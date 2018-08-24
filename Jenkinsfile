pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Hello Jenkins') {
      steps {
        echo "Hello ${params.Name}!"
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
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}