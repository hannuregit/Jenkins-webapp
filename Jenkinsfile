pipeline {
    agent any

    stages {
        stage('SAST - OWASP Dependency-Check') {
            steps {
                echo 'Running OWASP Dependency-Check for index.html'

                // Run OWASP Dependency-Check using the Jenkins plugin
                dependencyCheck additionalArguments: '', 
                               installation: 'OWASP Dependency-Check',  // Name of the OWASP Dependency-Check installation in Jenkins
                               pattern: '**/*.html',  // Assuming index.html is in the root of your repository
                               reportsDirectory: 'dependency-check-report',  // Directory to store the report
                               skipped: false
            }
        }
    }
}
