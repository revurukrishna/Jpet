pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/revurukrishna/Jpet.git'
      }
    }
    stage('Build') {
      steps {
        sh 'mvn clean install'
      }
    }
    stage('Deploy') {
      steps {
        sh 'cp target/my-app.jar /opt/my-app/'
      }
    }
  }
}
