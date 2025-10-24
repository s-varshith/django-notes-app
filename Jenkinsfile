pipeline {
    agent {label "agent-1"}

    stages {
        stage('Clone') {
            steps {
                git url: "https://github.com/s-varshith/django-notes-app.git", branch: "main"
            }
        }
        stage('docker') {
            steps{
                sh 'docker build --pull -t notes-app:latest .'
            }
        }
        stage('deploy') {
            steps{
                sh 'docker compose up -d'
            }
        }
    }
}
