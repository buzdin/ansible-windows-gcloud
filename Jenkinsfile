pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh './gradlew'
            }
        }
        stage('Deploy') {
            steps {
                dir('ansible') {
                    sh './deploy.sh'
                }
            }
        }
    }
}