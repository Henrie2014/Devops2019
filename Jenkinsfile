pipeline {
  agent any
  tools {
     maven 'M2_HOME' 
  }
  environment {
    registry = "kserge2001/devops-pipeline"
    registrycredential = 'dockerhub'
  }
  stages {
    stage('Build'){
      steps {
        sh 'mvn clean'
        sh 'mvn install'
        sh 'mvn package'
      }
    }    
     stage('Test'){
      steps {
        echo "test step"
        sh 'mvn test'
      }
     }
     stage('Deploy'){
      steps {
        echo "deploy step"
        
       }
     }    
  }


