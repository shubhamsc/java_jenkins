pipeline {
    agent { docker { image 'maven:3.6.0' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn clean test-compile gauge:execute -DspecsDir=specs -Denv=firefox'
            }
        }
    }
}