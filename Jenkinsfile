pipeline {
  agent any
  stages {
    stage('Build') {
      when {
        beforeAgent true;
        anyOf {
          branch 'main';
          tag 'release-*';
        }
      }
      stages {
        stage("Checkout Branch") {
          steps {
            git(url: 'https://github.com/congminh090800/docker-hello-world', branch: 'main', changelog: true)
          }
        }
        stage('See workplace') {
          steps {
            bat 'echo branch name: %BRANCH_NAME%'
            bat 'echo change branch: %CHANGE_BRANCH%'
            bat 'echo change target: %CHANGE_TARGET%'
            bat 'echo tag name: %TAG_NAME%'
          }
        }
      }
    }
  }
}
