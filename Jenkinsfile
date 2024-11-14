pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Add build steps here, e.g., compiling code
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Simulate test execution (e.g., running unit tests)
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add deployment steps here, e.g., copying files to a server
            }
        }

        stage('Failing Stage') {
            steps {
                echo 'This stage will purposely fail...'
                // Purposefully fail this stage
                error 'Intentional failure in this stage!'
            }
        }
    }

    post {
        always {
            echo 'This will run after all stages, regardless of success or failure.'
        }
        success {
            echo 'This will run if the pipeline succeeds.'
        }
        failure {
            echo 'This will run if the pipeline fails.'
        }
    }
}
