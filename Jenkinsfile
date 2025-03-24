pipeline{
    agent any

    stages{
        stage('Cloning Github repo to Jenkins'){
            steps{
                scripts{
                    echo 'Cloning the Github repo to Jenkins.........'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github_token', url: 'https://github.com/HAllenT420/Hotel_Reservations_MLops.git']])
                }
            }
        }

    }
}