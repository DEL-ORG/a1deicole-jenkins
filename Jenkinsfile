pipeline {
agent any
    options {
        buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '3', numToKeepStr: '3'))
        disableConcurrentBuilds()
        timeout(time: 1, unit: 'HOURS')
        timestamps() // Corrected syntax here
    }

    stages {
        stage('Test') {
            steps {
                sh '''
                kubectl 
                pwd
                uname -r 
                touch eric
                '''
            }
        }
    }
}
