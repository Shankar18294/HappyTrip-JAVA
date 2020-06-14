pipeline {
     agent any {
          stages {
          
                stage('checkout') {
                step{
             checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '216e5c2e-1262-4284-b659-457d9f80b415', url: 'https://github.com/Shankar18294/HappyTrip-JAVA.git']]])
                     }
                                  }
                                  
             stage('Build') {
              step{
     echo 'building..'
    }
}

stage('Test') {
              step{
         echo 'testing..'
    }
}

stage('Archive') {
              step{
              archiveArtifacts arifacts: '**/*.war, **/*.jar'
    }
}

stage('Deploy') {
              step{
        echo 'deploying..'
    }
}

stage('SonarQude analysis') {
              step{
        echo '..'
    }
}

    }
  }
}


                                  
                    
