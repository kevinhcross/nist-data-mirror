pipeline {
  agent {
    node {
      label 'centos-7'
    }
    
  }
  stages {
    stage('build') {
      steps {
        sh 'maven clean'
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