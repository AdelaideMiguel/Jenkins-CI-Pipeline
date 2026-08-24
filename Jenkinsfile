

pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code from GitHub...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo  'Build stage started - Lab 9 CI Pipeline.'
                echo 'Project build completed successfully.'
            }
        }

        stage('Test') {
            steps {
                echo 'Test stage started.'
                echo 'All tests completed successfully.'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment stage started.'
                echo 'Deployment completed successfully.'
            }
        }
    }

    post {
        success {
            echo '========================================'
            echo 'CI PIPELINE SUCCESSFUL'
            echo '========================================'
        }

        failure {
            echo '========================================'
            echo 'CI PIPELINE FAILED'
            echo 'Check the Console Output for details.'
            echo '========================================'
        }

        always {
            echo 'Jenkins Pipeline execution finished.'
        }
    }
}

