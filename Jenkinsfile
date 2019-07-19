pipeline {
    agent any
    stages {
        stage('cleanup') {
            steps { 
                sh ' echo "Hi, How are you PA ?" '
                deleteDir()
            }
        }
        stage('checkout') {
            steps { 
                checkout([$class: 'GitSCM', branches: scm.branches, doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'source:dsa-dev1', url: 'https://source.developers.google.com/p/dsa-dev1/r/pdz-ui']]])
            }
        }
    }
}
