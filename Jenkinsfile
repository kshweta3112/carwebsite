pipeline {
    agent any

    stages {

       stage('Clone') {
    steps {
        git branch: 'main', url: 'https://github.com/kshweta3112/carwebsite.git'
    }
        }

        stage('Build') {
            steps {
                sh 'echo Build Successful'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}
