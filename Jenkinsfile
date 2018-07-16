pipeline {
  agent {
    node {
      label 'jdk8'
    }

  }
  stages {
    stage('Hello') {
      steps {
        echo "Hello ${MY_NAME}!"
        sh 'java -version'
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
      }
    }
  }
  environment {
    MY_NAME = 'yamini'
    TEST_USER = credentials('test-user')
  }
}