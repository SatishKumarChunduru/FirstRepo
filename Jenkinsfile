pipeline {
  agent any
  stages {
    stage('Welcome') {
      steps {
        echo 'Welcome to Blue Ocean'
      }
    }
    stage('Clean') {
      parallel {
        stage('Clean') {
          steps {
            bat 'mvn clean'
          }
        }
        stage('Post Clean') {
          steps {
            echo 'Clean Completed'
          }
        }
      }
    }
    stage('Install') {
      steps {
        bat 'mvn install'
      }
    }
  }
}