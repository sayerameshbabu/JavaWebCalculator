pipeline{
  agent any
  environment{
    ANSIBLE=credentials('ansible-server')
  }
  stages{
    stage("building"){
      steps{
        sh 'mvn install'
        sh 'mvn clean package'
        sh 'pwd'
      }
    }
    stage("transfering files"){
      steps{
        echo 'hi'
       // sh ' scp target/*.war ansadmin@172.31.55.146:/home/ansadmin/apache-tomcat-7.0.94/webapps/  '
      }
    }
  }
}
