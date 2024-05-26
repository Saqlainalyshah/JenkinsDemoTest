pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building App...'
                sh  'node --version'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing App...'
                sh 'node App.js'
                sh 'gcloud compute zones list'
                sh 'gcloud compute scp /var/lib/jenkins/workspace/Multibranch-Pipeline-project_main/index.html root@saqlain-appache-jenkins:/var/www/html --zone=us-central1-a'
            }
}
}
}
