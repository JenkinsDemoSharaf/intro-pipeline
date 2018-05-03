pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${MY_NAME}!"
        sh 'java -version'
        echo "Test User is ${TEST_USER_USR}"
        echo "Test password = ${TEST_USER_PSW}"
      }
    }
  }
  environment {
    MY_NAME = 'Mouhab'
    TEST_USER = credentials('test-user')
  }
}