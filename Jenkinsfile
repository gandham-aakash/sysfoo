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
  stages{
  
    stage('test'){
      steps{
        sh 'mvn clean test'
      }
    }
   stages{
  
    stage('package'){
      steps{
        sh 'mvn package -DskipTests'
      }
    }
  }
  
  
}
