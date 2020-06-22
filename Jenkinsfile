pipeline {
     agent any
     
          stages {
          
                stage('checkout') {
                steps{
             checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '216e5c2e-1262-4284-b659-457d9f80b415', url: 'https://github.com/Shankar18294/HappyTrip-JAVA.git']]])
                     }
                                  }
                                  
             stage('compile') {
                   tools {
        jdk 'jdk11'
        maven 'maven 3.6.3'
        }
              steps{
     powershell 'mvn -f happytrip-code/pom.xml compile'
    }
}

stage('package') {
              steps{
         powershell 'mvn -f happytrip-code/pom.xml package'
    }
}

stage('Archive') {
              steps{
              echo '..'
    }
}

stage('Deploy') {
              steps{
        echo 'deploying..'
    }
}

stage('SonarQude analysis') {
              steps{
        echo '..'
    }
}

    }
  }


                                  
                    
