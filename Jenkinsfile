pipeline {
    agent any

    stages {
        stage('build') {
            steps {
              node('build-server-label') {
                    // some block
                    sh 'curl -4 www.icanhazip.com'
                }  
            }
        }
        
    }
}
