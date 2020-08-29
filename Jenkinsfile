pipeline {
    options {
        buildDiscarder(logRotator(numToKeepStr: '10'))
        disableConcurrentBuilds()
    }
    
    agent { label 'master' }
    
    environment { 
        envVar = 'Beispiel Env Var'
    }
    
    stages {
        stage('Init') {
            steps {
                echo 'Init...'
                echo "build id:     ${env.BUILD_ID} "
                echo "jenkins url:  ${env.JENKINS_URL}"
                echo "build tag:    ${BUILD_TAG}"
                echo "env var:      ${envVar}"
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
