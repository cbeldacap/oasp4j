pipeline {
  agent any
  stages {
    stage('go to samples') {
      steps {
        dir(path: '/samples')
      }
    }
    stage('install dependencies') {
      steps {
        sh 'mvn install'
      }
    }
    stage('build artifact') {
      steps {
        sh 'mvn package'
      }
    }
  }
}