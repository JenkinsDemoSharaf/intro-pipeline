pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${MY_NAME}!"
        sh 'java -version'
        echo "${TEST_USER_USR}"
      }
    }
  }
  environment {
    MY_NAME = 'Mouhab'
    TEST_USER = credentials('test-user')
  }
}