pipeline {
  agent any
  stages {
    stage('Git Checkout ') {
      steps {
        git(url: 'https://github.com/congminh090800/docker-hello-world', branch: 'main', changelog: true)
      }
    }

    stage('See workplace') {
      steps {
        bat 'dir'
      }
    }

  }
}