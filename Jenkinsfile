pipeline {
  agent any
  stages {
    stage('build clean') {
      parallel {
        stage('build clean') {
          steps {
            echo 'Build clean'
            sh 'mvn clean'
          }
        }
        stage('build deploy') {
          steps {
            echo 'Hello deploy stage'
          }
        }
      }
    }
    stage('Build Package') {
      steps {
        echo 'Build packaging'
        sh 'mvn package'
      }
    }
    stage('Build install') {
      steps {
        echo 'build install'
        sh 'mvn install'
      }
    }
  }
}