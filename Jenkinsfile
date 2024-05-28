pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building App...'
                sh  'node --version'
            }
        }
        stage('Deploying') {
            steps {
                echo 'Deploying App...'
                sh 'node App.js'
               //sh 'gcloud compute zones list'
                sh 'gcloud compute scp /var/lib/jenkins/workspace/assignment_main/index.html root@saqlain-appache-jenkins:/var/www/html --zone=us-central1-a'
                sh 'gcloud compute scp /var/lib/jenkins/workspace/assignment_main/about.html root@saqlain-appache-jenkins:/var/www/html --zone=us-central1-a'
                sh 'gcloud compute scp /var/lib/jenkins/workspace/assignment_main/contact.html root@saqlain-appache-jenkins:/var/www/html --zone=us-central1-a'
                sh 'gcloud compute scp /var/lib/jenkins/workspace/assignment_main/projects.html root@saqlain-appache-jenkins:/var/www/html --zone=us-central1-a'

            }
}
}
}
