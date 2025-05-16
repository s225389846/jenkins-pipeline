pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                script {
                    echo "Building the application..."
                }
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                script {
                    echo "Running unit tests..."
                }
            }
        }
        stage('Code Analysis') {
            steps {
                script {
                    echo "Analyzing code quality..."
                }
            }
        }

        // Stage 4: Security Scan
        stage('Security Scan') {
            steps {
                script {
                    echo "Performing security scan..."
                }
            }
        }

        stage('Deploy to Staging') {
            steps {
                script {
                    echo "Deploying to staging environment..."
                }
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                script {
                    echo "Running integration tests on staging..."
                }
            }
        }

        stage('Deploy to Production') {
            steps {
                script {
                    echo "Deploying to production..."
                }
            }
        }
    }

    post {
        always {
            echo "Pipeline completed."
        }

        success {
            echo "Pipeline completed successfully!"
        }

        failure {
            echo "Pipeline failed. Please check the logs."
        }
    }
}
