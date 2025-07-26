pipeline {
    agent any

    tools {
        // This name MUST EXACTLY MATCH the name you set in Jenkins
        maven 'Maven-3.9.11'
    }

    stages {
        stage('Checkout Code') {
            steps {
                // Get the code from your GitHub repository
                git 'https://github.com/OCT0619/springboot-jenkins-project.git'
            }
        }
        stage('Build Project') {
            steps {
                // Run the Maven command to build the project
                sh 'mvn clean install'
            }
        }
    }
}
