pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building App...'
                sh "node app.js"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing App...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying App...'
            }
        }
    }
}
