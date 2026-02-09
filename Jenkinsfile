pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/<username>/jenkins-terraform-project.git'
            }
        }

        stage('Build') {
            steps {
                echo "Build stage completed"
            }
        }

        stage('Test') {
            steps {
                echo "Test stage completed"
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo mkdir -p /var/www/html
                sudo cp app/index.html /var/www/html/index.html
                '''
            }
        }
    }
}
