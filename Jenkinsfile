pipeline {
     agent any
     
          stages {
          
                stage('checkout') {
                steps{
             checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '216e5c2e-1262-4284-b659-457d9f80b415', url: 'https://github.com/Shankar18294/HappyTrip-JAVA.git']]])
                     }
                                  }
                                  
             stage('Build') {
              steps{
     echo 'building..'
    }
}

stage('Test') {
              steps{
         echo 'testing..'
    }
}

stage('Archive') {
              steps{
              archiveArtifacts arifacts: '**/*.war, **/*.jar'
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


                                  
                    
