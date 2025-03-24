pipeline{
    agent any

    environment {
        VENV_DIR = 'venv'
        
    }

    stages{
        stage('Cloning Github repo to Jenkins'){
            steps{
                script{
                    echo 'Cloning the Github repo to Jenkins.........'
                    checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github_token', url: 'https://github.com/HAllenT420/Hotel_Reservations_MLops.git']])
                }
            }
        }

        stage('Setting up our Virtual Environment and Installing Dependancies'){
            steps{
                script{
                    echo 'Setting up our Virtual Environment and Installing Dependancies.........'
                    sh '''
                    python -m venv ${VENV_DIR}
                    . ${VENV_DIR}/bin/activate
                    pip install --upgrade pip
                    pip install -e .
                    '''

                    
                }
            }
        }

    }
}
