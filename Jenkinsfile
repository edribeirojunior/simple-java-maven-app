pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/edribeirojunior/simple-java-maven-app', branch: 'master')
      }
    }
  }
}