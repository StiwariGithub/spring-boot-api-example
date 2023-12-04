pipeline {
    agent any

    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                chmod +x ./gradlew
                sh 'chmod + ./gradlew assemble'
            }
        }
        stage('Test') {
            steps {
                chmod +x ./gradlew
                sh 'chmod + ./gradlew test'
            }
        }
    }
}
