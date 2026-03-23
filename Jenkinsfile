pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Fetching code from GitHub...'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo rm -rf /var/www/html/*
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}
