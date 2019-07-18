pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'docker --version'
                sh 'mvn test-compile gauge:execute -DspecsDir=specs -Denv=firefox'
            }
        }
    }
}
