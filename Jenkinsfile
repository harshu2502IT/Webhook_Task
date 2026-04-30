pipeline {
    agent any
    stages {
        stage('Hello World') {
            steps {
                echo 'Hello from StayHub Webhook_Task!'
                echo 'This is your first Jenkins Pipeline 🎉'
            }
        }
        
        stage('Deploy to XAMPP') {
            steps {
                echo 'Copying files to htdocs...'
                bat 'xcopy /E /Y /I "%WORKSPACE%\\*" "C:\\xampp\\htdocs\\Webhook_Task\\"'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running basic tests...'
                bat 'dir'
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
