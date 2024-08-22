pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                // Fetch code from the specified Git repository
                git branch: 'master', url: 'https://github.com/hannuregit/Jenkins-webapp.git'
            }
        }
    }

    post {
        success {
            echo 'Code successfully fetched from the repository!'
        }
        failure {
            echo 'Failed to fetch the code from the repository.'
        }
    }
}
