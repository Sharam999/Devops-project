pipeline {
    agent any

    stages {
        stage('Verify Jenkins') {
            steps {
                echo 'Jenkins is working successfully!'
                sh 'whoami'
                sh 'java -version'
            }
        }

        stage('Checkout Website') {
            steps {
                echo 'Website source code will be checked out by Jenkins.'
                sh 'ls -la'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check Console Output for details.'
        }
    }
}
