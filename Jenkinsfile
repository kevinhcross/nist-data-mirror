pipeline {
  agent {
    node {
      label 'centos-7'
    }
    
  }
  tools {
    maven 'Maven_3.3.3'
    jdk 'JDK_8u111'
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
