pipeline {
    
    agent { label 'master' }
    
    environment { 
        CC = 'clang'
    }
    
    stages {
        stage('Init') {
            steps {
                echo 'Init...'
                echo "build id:     ${env.BUILD_ID} "
                echo "jenkins url:  ${env.JENKINS_URL}"
                echo "build tag:    ${BUILD_TAG}"
                sh 'mvn --version'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
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
