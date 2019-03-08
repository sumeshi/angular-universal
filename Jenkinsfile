pipeline {
    agent { docker 'trion/ng-cli-e2e' }
    stages {
        stage('setup') {
            steps {
                sh 'npm install'
            }
        }
        stage('build') {
            steps {
                sh 'ng e2e'
            }
        }
    }
}
