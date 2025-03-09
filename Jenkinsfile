pipeline {
    agent any  // Runs on any available Jenkins agent

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-repo/my-html-project.git'
            }
        }

        stage('Build') {
            steps {
                script {
                    echo "No build required for HTML & CSS project"
                }
            }
        }

        stage('Deploy') {
            steps {
                sh 'mkdir -p /var/www/html/my-html-project'
                sh 'cp -r * /var/www/html/my-html-project/'
            }
        }

        stage('Post-Build') {
            steps {
                echo 'Deployment Completed!'
            }
        }
    }
}
