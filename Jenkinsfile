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
                sh 'gcloud compute zones list'
                echo "This is my IP"
                curl -s ifconfig.co
                echo "This is my hostname"
                hostname -f

            }
}
}
}
