pipeline {
    agent {
        label 'jenkins-slave-node'
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test'){
            steps {
                sh 'npm run start:dev'
            }
        }
       
    }
}
