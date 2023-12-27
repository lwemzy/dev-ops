pipeline {
    agent {
        node {
            label 'docker_agent_alpine'
        }
    }
    triggers {
        pollSCM '*/5 * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh '''
                echo "doing build stuff"
                '''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh '''
                echo "doing test stuff"
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver...'
                sh '''
                echo "doing deliver stuff"
                '''
            }
        }
    }
}
