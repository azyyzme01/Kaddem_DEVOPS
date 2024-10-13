pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Correct Git checkout syntax
                git url: 'https://github.com/azyyzme01/Kaddem_DEVOPS.git', branch: 'main'
            }
        }
        stage('Build Backend') {
            steps {
                // Add your backend build steps here
                echo 'Building Backend...'
            }
        }
        stage('Build Frontend') {
            steps {
                // Add your frontend build steps here
                echo 'Building Frontend...'
            }
        }
        // Add more stages as needed...
    }
}
