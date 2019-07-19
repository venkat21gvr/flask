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
                checkout scm
            }
        }
    }
}
