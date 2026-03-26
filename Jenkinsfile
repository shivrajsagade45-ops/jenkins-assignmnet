pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/shivrajsagade45-ops/jenkins-assignmnet.git'
            }
        }

        stage('Deploy to Apache') {
            steps {
                sh '''
                sudo cp index.html /var/www/html/
                sudo systemctl restart httpd
                '''
            }
        }

    }
}
