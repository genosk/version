pipeline {
    agent any
    environment {
        MY_ENV_VAR = 'value'
    }
    stages {
        stage('Checkout') {
            steps {
                // Checkout code from Git repository using credentials
                git credentialsId: 'genosk', url: 'https://github.com/genosk/version.git'
            }
        }
        // Other stages (Build, Test, Deploy)
    }
}
