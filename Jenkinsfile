pipeline{
  agent any
  stages {
    stage('Compile stage') {
      steps {
        withMaven(maven : maven_3.8.1) {
        sh 'mvn clean compile'
        }
      }
    }
    stage('Testing stage'){
      steps {
        withMaven(maven : maven_3.8.1) {
        sh 'mvn test'
        }
      }
    }
    stage('Deploy stage'){
      steps {
        withMaven(maven : maven_3.8.1) {
        sh 'mvn deploy'
        }
      }
    }
        
