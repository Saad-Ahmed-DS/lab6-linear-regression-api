pipeline {
    agent any
    triggers {
        githubPush()
    }
    stages {
        stage('Deploy API') {
            steps {
                sh 'docker compose pull'
                sh 'docker compose up -d'
            }
        }
    }
}
