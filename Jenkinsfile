pipeline {
  agent any
  stages {
    stage('Git Checkout ') {
      steps {
        git(url: 'https://github.com/congminh090800/docker-hello-world', branch: 'main')
      }
    }

    stage('See workplace') {
      steps {
        bat 'echo %BRANCH_NAME% %CHANGE_TITLE%  %CHANGE_ID% %CHANGE_TARGET% %CHANGE_BRANCH% '
      }
    }

  }
}