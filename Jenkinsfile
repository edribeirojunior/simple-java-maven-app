pipeline {
  agent {
    docker {
          image 'maven:3-alpine'
    }
  }
  stages {
    stage('SCM') {
      steps {
        git(url: 'https://github.com/edribeirojunior/simple-java-maven-app', branch: 'master')
      }
    }
    stage('Build') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }
  }
}
