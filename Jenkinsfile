pipeline{
  agent any
  stages{
    stage("building"){
      steps{
        sh 'mvn install'
        sh 'mvn clean package'
        sh 'pwd'
      }
    }
  }
}
