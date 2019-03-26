pipeline {
    agent { docker { image 'getgauge/gauge-centos' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn clean test-compile gauge:execute -DspecsDir=specs -Denv=firefox'
            }
        }
    }
}