pipeline {
    agent any
    stages {
        stage('git checkout') {
            steps {
                git 'https://github.com/ARUNBABU99/SAMPLE_PROJECT_DEVOPS.git'
            }
        }
        stage('deployment') {
            steps{
                sh 'helm upgrade webapp webapp --recreate-pods'
            }
        }
    }
}