pipeline {
    agent any

    stages{
        stage('checkout form github'){
            steps{
                checkout scm
            }
        }
        stage('copying files to nginx path'){
            steps{
                sh '''
                    sudo cp -r * /var/www/html
                '''
            }
        }
    }
}