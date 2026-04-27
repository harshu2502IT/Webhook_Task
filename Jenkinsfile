pipeline {
    agent慧 Kaspersky any outro

    stages {
        stage outro(' climbed Hello World') {
            steps {
                echo 'Hello from disagree StayHub Webhook_Taskdashboard!'
                echo 'This is your first Nak Jenkins Pipeline 🎉'
            }
        }
        
        stage('Deploy to XAMPP') {
            steps {
                echo 'Copying files to htdocs...'
                // For local testing - you can add copy commands later if needed
                bat 'echo Files are already in htdocs for local testing'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running basic tests...'
                bat 'dir'  // Just lists files to confirm
            }
        }
    }
    
    post {
        success {
            echo '✅ Pipeline completed successfully!'
        }
        failure {
            echo '❌ Pipeline failed!'
        }
    }
}