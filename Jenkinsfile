pipeline {
    
    agent { label 'master' }
    
    stages {
        stage('Init') {
            steps {
                echo 'Init...'
                echo "build id:    ${env.BUILD_ID} "
                echo "jenkins url: ${env.JENKINS_URL}"
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                echo "build tag: ${BUILD_TAG}"
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
