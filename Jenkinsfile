pipeline {
    
    agent { label 'master' }
    
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                echo "build tag: ${BUILD_TAG}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
