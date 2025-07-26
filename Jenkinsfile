pipeline {
    agent any

    tools {
        // This name MUST EXACTLY MATCH the name you set in Jenkins
        maven 'Maven-3.9.11'
    }

    stages {
        stage('Build Project') {
            steps {
                // Run the Maven command to build the project
                sh 'mvn clean install -DskipTests'
            }
        }
    }
}
