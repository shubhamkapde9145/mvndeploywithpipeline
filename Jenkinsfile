pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git branch: 'dependabot/maven/junit-junit-4.13.1', url: 'https://github.com/Girish-154/simpleMavenJunit.git'

    
                sh 'mvn clean'
                sh 'mvn test'
                sh 'mvn compile'
                sh 'mvn package'
            }

         
            }
        }
    }
