pipeline {
    agent any

    stages {
        stage('Build Application') {
            steps {
                bat 'mvn clean install'
            }
        }
        stage('Test Application') {
            steps {
                bat 'mvn clean test'
            }
        }
        stage('Deploy Application') {
            steps {
                bat 'mvn deploy package'
            }
        }
    }
}