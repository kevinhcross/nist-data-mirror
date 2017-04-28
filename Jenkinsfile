pipeline {
  agent {
    node {
      label 'centos-7'
    }
    
  }
  stages {
    stage('build') {
      steps {
        tool(name: 'Maven_3.0.5', type: 'Maven_3.0.5')
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