pipeline {
    agent any
    stages {
        stage('get awscli access') {
            steps {
                sh "aws sts get-caller-identity"
            }
        }
        stage('delete eks cluste') {
            steps {
                sh "ekscli delete-cluster --name ezlearn-cluster"
            }
        }
    }
}
