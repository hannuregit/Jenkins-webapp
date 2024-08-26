pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from your repository
                git branch: 'master', url: 'https://github.com/hannuregit/Jenkins-webapp.git'
            }

            
        }
        stage('testing'){
            
            steps {
            echo "hello world"
    }
  }
}

post {
  always {
    echo "i am gonna run every single time"
  }
  failure {
    echo "only when something fails"
  }
  success {
    echo "this section will execute when everything is fine"
  }
 }
}   
    
    
        
        
    

    
