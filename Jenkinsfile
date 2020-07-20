pipeline{
  
  agent any
  
  tools{
    maven 'M2_HOME'
  }
  
  stages{
  
    stage('build'){
      steps{
        sh 'mvn compile'
      }
    }
  
    stage('test'){
      steps{
        sh 'mvn clean test'
      }
    }
  
    stage('package'){
      steps{
        sh 'mvn package -DskipTests'
      }
    }
  }
  
  
}
