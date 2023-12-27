pipeline {
    agent {
        node {
            label 'docker_agent_alpine'
        }
    }
    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh '''
                echo "Runing Java Main application"
                java Main.java
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
