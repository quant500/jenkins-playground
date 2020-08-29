pipeline {
    
    agent { label 'master' }
    
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                echo BUILD_TAG
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
