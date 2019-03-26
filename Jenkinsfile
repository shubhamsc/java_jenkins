pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn test-compile gauge:execute -DspecsDir=specs -Denv=firefox'
            }
        }
    }
}