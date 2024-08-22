pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from your repository
                git branch: 'master', url: 'https://github.com/hannuregit/Jenkins-webapp.git'
            }
        }

        
        }

        stage('Run Script') {
            steps {
                // Run the hello_world.py script
                sh 'python3 hello_world.py'
            }
        }
    

    post {
        success {
            echo 'Python script executed successfully!'
        }
        failure {
            echo 'Failed to execute Python script.'
        }
     }    
    
}
