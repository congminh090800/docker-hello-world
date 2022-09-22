pipeline {
  agent any
  stages {
    stage('Git Checkout ') {
      steps {
        git(url: 'https://github.com/congminh090800/docker-hello-world', branch: 'main')
      }
    }

    stage('Print dir') {
      steps {
        sh 'ls -a'
      }
    }

  }
}