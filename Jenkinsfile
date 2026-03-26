pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/YOUR_USERNAME/YOUR_REPO.git'
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
