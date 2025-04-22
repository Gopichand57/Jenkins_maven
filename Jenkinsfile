pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the repository
                git branch: 'main', url: 'https://github.com/Gopichand57/Jenkins_maven.git'
            }
        }
        
        stage('Build') {
            steps {
                // Run Maven build
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Run Maven test
                sh 'mvn test'
            }
        }
    }
}
