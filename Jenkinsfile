pipeline {
  agent any
  stages {
    stage('checkout ') {
      steps {
        git(url: 'https://github.com/jfrog/project-examples.git', branch: 'master')
      }
    }

    stage('build') {
      steps {
        sh 'mvn clean install'
      }
    }

  }
}