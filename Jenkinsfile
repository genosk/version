pipeline {
    agent any
    
    environment {
        MY_ENV_VAR = 'value' // Optional environment variable
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code from Git repository'
                git 'https://github.com/genosk/version.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // Replace this with your actual build command
                sh 'mvn clean install' // For Maven project
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Replace this with your actual test command
                sh 'mvn test' // For Maven projects
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to server...'
                // Replace this with your actual deploy command
                sh 'deploy_to_server.sh' // Example deploy command
            }
        }
    }
}
