pipeline {
    agent {label "agent-1"}

    stages {
        stage('Clone') {
            steps {
                git url: "https://github.com/s-varshith/django-notes-app.git", branch: "main"
            }
        }
    }
}
