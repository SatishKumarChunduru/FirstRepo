pipeline {
  agent any
  stages {
    stage('Start Message') {
      steps {
        echo 'Welcome to Blue Ocean'
      }
    }
    stage('Clean') {
      steps {
        bat 'mvn clean'
      }
    }
    stage('End Message') {
      steps {
        echo 'Succesfully Cleaned !!'
      }
    }
  }
}