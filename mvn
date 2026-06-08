pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
stage('Debug') {
    steps {
        sh 'whoami'
        sh 'echo $PATH'
        sh 'which mvn'
        sh 'mvn -version'
    }
}
}
