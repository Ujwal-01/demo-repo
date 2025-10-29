pipeline {
    agent any

    environment {
        // Reference Jenkins credential ID (you’ll create this in Jenkins)
        GIT_CREDENTIALS_ID = 'a181863c-a1b1-4001-98ae-f2ff14df3261'
        GIT_REPO_URL = 'https://github.com/Ujwal-01/demo-repo.git'
    }

    stages {
        stage('Checkout') {
            steps {
                echo "Checking out the latest code from GitHub repo..."
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Running build stage..."
                sh 'echo "Build successful!"'
            }
        }

        stage('Test') {
            steps {
                echo "Running test cases..."
                sh 'echo "All tests passed!"'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying the application..."
                sh 'echo "Deployment completed successfully!"'
            }
        }
    }

}
