pipeline {
    agent any
    tools {
        nodejs 'NodeJs'
    }
    stages {
        stage ('chechout from git hub')  {
            steps {
               git branch: 'main', credentialsId: 'GIT-HUB-ACCESS-TOKEN', url: 'https://github.com/ABBEYOWO/pipeline-docker-k8.git'
            }
        }
        stage ('install node depenedencies')  {
            steps {
                sh 'npm install'
            }
        }
        stage ('test node')  {
            steps {
                 sh 'npm test'
            }
        }
        stage ('configure')  {
            steps {
               echo "configure"
            }
        }
    }
}

