pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                echo "Cloning repository..."
                checkout scm
            }
        }

        stage('Build Stage') {
            steps {
                echo "Build step running..."
            }
        }

        stage('Test Stage') {
            steps {
                echo "Running simple tests..."
            }
        }

        stage('Deploy Stage') {
            steps {
                echo "Deployment simulated!"
            }
        }
    }

    post {
        success {
            echo "Pipeline completed successfully ✅"
        }
        failure {
            echo "Pipeline failed ❌"
        }
    }
}
