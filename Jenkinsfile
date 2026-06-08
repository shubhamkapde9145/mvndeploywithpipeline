pipeline {
    agent any

    tools {
        jdk 'JDK17'
        maven 'Maven'
    }

    stages {

        stage('Debug') {
            steps {
                sh 'java -version'
                sh 'mvn -version'
                sh 'which java'
                sh 'which mvn'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

    }

    post {
        success {
            echo 'Build Successful'
        }
        failure {
            echo 'Build Failed'
        }
    }
}
