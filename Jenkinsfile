pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from GitHub
                git url: 'https://github.com/azyyzme01/Kaddem_DEVOPS.git', branch: 'main' // Adjust branch name if needed
            }
        }

        stage('Build Backend') {
            steps {
                // Build the backend (Spring) using Maven
                sh 'cd backend && mvn clean install'
            }
        }

        stage('Build Frontend') {
            steps {
                // Build the frontend (Angular) using Maven
                sh 'cd frontend && mvn clean install'
            }
        }
    }

    post {
        success {
            echo 'Build completed successfully!'
        }
        failure {
            echo 'Build failed.'
        }
    }
}
