pipeline {
    agent any
    stages {
        stage ('chechout from git hub')  {
            steps {
               git branch: 'main', credentialsId: 'GIT-HUB-ACCESS-TOKEN', url: 'https://github.com/ABBEYOWO/pipeline-docker-k8.git'
            }
        }
        stage ('testing')  {
            steps {

            }
        }
        stage ('edit')  {
            steps {

            }
        }
        stage ('configure')  {
            steps {

            }
        }
    }
}
