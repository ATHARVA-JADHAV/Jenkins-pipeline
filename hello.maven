pipeline {
    agent any
    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "Maven 3.9.5"
    }
    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/ATHARVA-JADHAV/Jenkins-pipeline.git'
            }
        }
        stage('Build Code') {
            steps {
                bat "mvn clean install"
            }
        }
    }
}
