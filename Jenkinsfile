pipeline {
    agent any
    triggers { cron('H H(18-19) * * *') }
    options { 
        buildDiscarder(logRotator(daysToKeepStr: '30', numToKeepStr: '100') ) 
        disableConcurrentBuilds()
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Build"'
            }
        }
    }
}
