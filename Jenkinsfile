pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'chmod +x mvnw'
                sh './mvnw clean package'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh './mvnw test'
            }
        }
    }
}
