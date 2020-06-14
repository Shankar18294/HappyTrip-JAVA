pipeline {
     agent any {
             tools {
                 //jdk "Java-11"
                 //maven "maven 3.6.3"
                  }
                  
          stages {
          
                stage('checkout') {
                step{
             checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '216e5c2e-1262-4284-b659-457d9f80b415', url: 'https://github.com/Shankar18294/HappyTrip-JAVA.git']]])
                     }
                                  }
                                  
             stage('Build') {
              step{
    // some block
    }
}

stage('Build') {
              step{
    // some block
    }
}

stage('Test') {
              step{
         echo 'building..
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


                                  
                    
