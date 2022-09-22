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
        bat 'echo %env.BRANCH_NAME% %env.CHANGE_TARGET% %env.CHANGE_BRANCH% '
      }
    }

  }
}