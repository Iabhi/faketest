pipeline {
    agent any
    stages {
        stage('Approval') {
            steps {
                // Pauses execution until a user clicks "Proceed" or "Abort"
                input message: "Ready to deploy to Production?", ok: "Deploy!"
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying..."
            }
        }
    }
}