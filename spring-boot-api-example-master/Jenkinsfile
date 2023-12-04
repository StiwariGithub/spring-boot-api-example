pipeline {
    agent any

    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                sh 'chmod + ./gradlew assemble'
            }
        }
        stage('Test') {
            steps {
                sh 'chmod + ./gradlew test'
            }
        }
    }
}
