pipeline {
  agent {
    node {
      label 'centos-7'
    }
    
  }
  stages {
    stage('build') {
      steps {
        sh 'mvn clean'
        sh 'mvn compile'
      }
    }
    stage('test') {
      steps {
        sh 'mvn test'
      }
    }
  }
}