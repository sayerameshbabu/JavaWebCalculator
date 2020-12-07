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
        sh ' sudo scp -i /home/ec2-user/.ssh/id_rsa target/*.war centos@172.31.55.146:/home/centos/  '
      }
    }
  }
}
