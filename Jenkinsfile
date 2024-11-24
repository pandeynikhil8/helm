pipeline {
    agent any // Use any available agent
    stages {
        stage('Checkout Code') {
            steps {
                // Clone the Git repository (uses configured credentials if needed)
                git branch: 'main', url: 'git@github.com:your-repo/your-project.git'
            }
        }
        stage('Build') {
            steps {
                // Build your project (replace with your actual build command)
                sh 'echo "Building project..."'
            }
        }
        stage('Print Directory Structure') {
            steps {
                // List the directory structure
                sh 'ls -la'
            }
        }
    }
    post {
        always {
            // Always clean up workspace after the build
            cleanWs()
        }
    }
}