pipeline {
    agent any
    stages {
        stage ('check out git'){
            steps {
               git branch: 'main', credentialsId: 'GIT-HUB-ACCESS-TOKEN', url: 'https://github.com/ABBEYOWO/pipeline-docker-k8.git'
            }
        }
        stage ('install node dependencies'){
            steps {
              echo 'installing'
            }
        }
        stage ('test code'){
            steps {
              echo 'tessting'
            }
        }
        
    }
    post {
        success {
            echo 'build completed successfully'
        }
        failure {
            echo 'this build has failed'
        }
    }
}
